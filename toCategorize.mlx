function toCategorize = CategorizeData(toCategorize, categories)

for x = 1:length(toCategorize)
    str = string(toCategorize(x));
    
    % Check str against typeCats: If substring is found, assign MaterialType at x 
    % to that category and continue 
    for item = categories
        if contains(str,item)
            toCategorize(x) = categorical(item);
            continue
        end
    end
    
    % If MaterialType at x is not a defined category, assign it to other
    if ~(any(categories(:) == string(toCategorize(x))))
        toCategorize(x) = categorical("Other");
    end
end

toCategorize = removecats(toCategorize);

end
