# assignment2-taidala

# Navyapreethi Taidala
###### victoria Falls
>victoria Falls (Lozi: Mosi-oa-Tunya, "The Smoke That Thunders"; Tonga: Shungu Namutitima, "Boiling Water") is a waterfall on the Zambezi River in southern Africa, which provides habitat for several unique species of plants and animals. It is located on the border between Zambia and Zimbabwe and is one of the world's largest waterfalls, with a width of 1,708 m (5,604 ft).
David Livingstone, the Scottish missionary and explorer, is believed to have been the first European to view the falls on 16 November 1855, from what is now known as **Livingstone Island**, one of two land masses in the middle of the river, immediately upstream from the falls near the Zambian shore.<br> Livingstone named his sighting in honour of **Queen Victoria**, but the Sotho language name, Mosi-oa-Tunya—"The Smoke That Thunders"—continues in common usage. The World Heritage List officially recognises both names.
---
## Directions from Maryville to Victoria Falls
1. First travelling to Kansas city from Maryville through car.
2. From Kansas city take a flight to Zambia,Johannesburg. 
3. After arriving in Johannesburg, we’d then have to catch a connecting flight to the closest airports to Victoria Falls.
  1. When we made our visit in late May 2008, the country of Zimbabwe was undergoing some political turmoil, which made it too risky to fly to the Victoria Falls airport. That flight would have taken us under 2 hours.
  2. Instead, we wound up flying from Johannesburg to Livingstone, Zambia. That flight took us under 2 hours. However, the distance between Livingstone and the actual waterfall itself was around 11km, which was a bit much for a walk. So we had to take a taxi there.
  3. On the other hand, had we been able to fly right into the town of Victoria Falls, Zimbabwe, then we conceivably could have been transported to the main part of town, then literally walk 2km or so to the actual waterfall itself.
  4. A luxury dinner train crosses from Zambia to Zimbabwe over the Zambezi River and stops in the middle for a view of the Falls (though plans call for an additional departure in the other direction). For an aerial view, microlight flights are popular, and so is bungee jumping.
4. Reached destination of Victoria Falls now you can enjoy scenario of great Water Falls in the World.
   * Things need to bring for my favourite  destination
* clothes
* food
* snacks
* drinks
* water
* coke

**[Link to AboutMe.md](AboutMe.md)**

***

# Editing table for popular foods that present in different places
I like different kinds of spicy foods.A food is something that provides nutrients. Nutrients are substances that provide: energy for activity, growth, and all functions of the body such as breathing, digesting food, and keeping warm.

| Types of food   | place     | price of food |
| ---             | ---       | ---:          |
| chicken biryani | hyderabad | 600 rupees    |
| Dhokla khandvi  | gujatat   | 500 rupees    |
| Mutton curry    | hyderabad | 800 rupees    |

***

# Quotes to inspire in daily life

> Your time is limited, so don't waste it living someone else's life. Don't be trapped by dogma – which is living with the results of other people's thinking. -Steve Jobs

> If you look at what you have in life, you'll always have more. If you look at what you don't have in life, you'll never have enough.-Oprah Winfrey

***

# code Fencing
> Bipartite Graph check is an algorithm in the mathematical field of graph theory, a bipartite graph (or bigraph) is a graph whose vertices can be divided into two disjoint and independent sets {\displaystyle U}U and {\displaystyle V}V such that every edge connects a vertex in {\displaystyle U}U to one in {\displaystyle V}V. Vertex sets {\displaystyle U}U and {\displaystyle V}V are usually called the parts of the graph. Equivalently, a bipartite graph is a graph that does not contain any odd-length cycles.
Discover More in <https://en.wikipedia.org/wiki/Bipartite_graph>
~~~
> int n;
vector<vector<int>> adj;

vector<int> side(n, -1);
bool is_bipartite = true;
queue<int> q;
for (int st = 0; st < n; ++st) {
    if (side[st] == -1) {
        q.push(st);
        side[st] = 0;
        while (!q.empty()) {
            int v = q.front();
            q.pop();
            for (int u : adj[v]) {
                if (side[u] == -1) {
                    side[u] = side[v] ^ 1;
                    q.push(u);
                } else {
                    is_bipartite &= side[u] != side[v];
                }
            }
        }
    }
}

cout << (is_bipartite ? "YES" : "NO") << endl;
~~~
More Info <https://cp-algorithms.com/graph/bipartite-check.html>