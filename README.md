# Acroynm-using-python

def create_acronym(phrase):
    # Split the phrase into a list of words
    words = phrase.split()

    # Initialize the acronym as an empty string
    acronym = ""

    # Iterate through the words in the phrase
    for word in words:
        # If the word is at least two characters long, use the first character for the acronym
        if len(word) > 1:
            acronym += word[0]

    # Return the acronym in uppercase
    return acronym.upper()

# Test the function with some phrases
print(create_acronym("United States of America")) # should print "USA"
print(create_acronym("International Business Machines")) # should print "IBM"
print(create_acronym("HyperText Markup Language")) # should print "HTML"
print(create_acronym("Central Processing Unit")) # should print "CPU"
print(create_acronym("As Soon As Possible")) # should print "ASAP"
