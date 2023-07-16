### Hi there  😊

Im Erik from Northern Virginia, I possess the ability to analyze complex problems and identify patterns or vulnerabilities in systems. I am driven by the goal of safeguarding organizations' sensitive data and critical assets, ensuring their resilience against cyber threats. I enjoy making a tangible impact by protecting organizations from cyber threats and preserving their operations and reputation.

![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=eriklauni&hide=contribs,prs)

### Hi there 👋, Erik Launi
![](https://github.com/eriklauni)

I made this project just for fun, it allows you to create nice and simple GitHub Readme files that you can copy/paste and use in your profile.

Skills: Azure/Python/Security Audits

- 🔭 I’m currently working on Google Cybersecurity Cert. 
- 🌱 I’m currently learning Northern, VA 
- 🤔 I’m looking for help with Coding 
- 💬 Ask me about Sports  
- 📫 How to reach me: Insta-elaw31 


[<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/github.svg' alt='github' height='40'>](https://github.com/eriklauni)  [<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/linkedin.svg' alt='linkedin' height='40'>](https://www.linkedin.com/in/https://www.linkedin.com/in/erik-launi-a859aaa3//)  [<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/instagram.svg' alt='instagram' height='40'>](https://www.instagram.com/elaw31/)  [<img src='https://cdn.jsdelivr.net/npm/simple-icons@3.0.1/icons/icloud.svg' alt='website' height='40'>](https://github.com/eriklauni)  

![GitHub Activity Graph](https://activity-graph.herokuapp.com/graph?username=eriklauni)  

![GitHub streak stats](https://streak-stats.demolab.com/?user=eriklauni)  

![Profile views](https://gpvc.arturio.dev/eriklauni)  

def merge_sort(arr):
    if len(arr) <= 1:
        return arr

    # Split the array in half
    mid = len(arr) // 2
    left_half = arr[:mid]
    right_half = arr[mid:]

    # Recursively sort both halves
    left_half = merge_sort(left_half)
    right_half = merge_sort(right_half)

    # Merge the sorted halves
    return merge(left_half, right_half)


def merge(left, right):
    merged = []
    left_index, right_index = 0, 0

    # Compare elements from both halves and merge them
    while left_index < len(left) and right_index < len(right):
        if left[left_index] < right[right_index]:
            merged.append(left[left_index])
            left_index += 1
        else:
            merged.append(right[right_index])
            right_index += 1

    # Append remaining elements, if any
    while left_index < len(left):
        merged.append(left[left_index])
        left_index += 1

    while right_index < len(right):
        merged.append(right[right_index])
        right_index += 1

    return merged


# Test the merge_sort function
arr = [7, 2, 1, 6, 8, 5, 3, 4]
sorted_arr = merge_sort(arr)
print(sorted_arr)
