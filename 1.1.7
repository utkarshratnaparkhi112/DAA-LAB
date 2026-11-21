#include <stdio.h>
#include <limits.h>

#define MAX 1000
#define INF 1000000000

typedef struct {
    int u;
    int v;
    int w;
} Edge;

Edge edges[MAX * MAX];
int dist[MAX + 1];
int parent[MAX + 1];

void printPath(int v) {
    if (parent[v] == -1) {
        printf("%d", v);
        return;
    }

    printPath(parent[v]);
    printf("->%d", v);
}

int main() {
    int V, E;
    int src;

    scanf("%d", &V);
    scanf("%d", &E);

    for (int i = 0; i < E; i++) {
        scanf("%d %d %d",
              &edges[i].u,
              &edges[i].v,
              &edges[i].w);
    }

    scanf("%d", &src);

    // Initialize distances and parents
    for (int i = 1; i <= V; i++) {
        dist[i] = INF;
        parent[i] = -1;
    }

    dist[src] = 0;

    // Bellman-Ford: V-1 relaxation rounds
    for (int i = 1; i <= V - 1; i++) {
        int changed = 0;

        for (int j = 0; j < E; j++) {
            int u = edges[j].u;
            int v = edges[j].v;
            int w = edges[j].w;

            if (dist[u] != INF && dist[u] + w < dist[v]) {
                dist[v] = dist[u] + w;
                parent[v] = u;
                changed = 1;
            }
        }

        if (!changed)
            break;
    }

    // Check for negative weight cycle
    for (int i = 0; i < E; i++) {
        int u = edges[i].u;
        int v = edges[i].v;
        int w = edges[i].w;

        if (dist[u] != INF && dist[u] + w < dist[v]) {
            printf("Negative cycle detected\n");
            return 0;
        }
    }

    // Print shortest distance and path
    for (int i = 1; i <= V; i++) {
        if (i == src)
            continue;

        if (dist[i] == INF) {
            printf("%d INF None\n", i);
        } else {
            printf("%d %d ", i, dist[i]);
            printPath(i);
            printf("\n");
        }
    }

    return 0;
}
