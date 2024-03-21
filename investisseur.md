Paul Raynaud

# Problème d'investissement original:
On cherche à maximiser le capital d'un investisseur au cours d'une plage de temps $x(t), t \in [0, T]$.
Le capital initial est $x(0)=x_0$.
Un investisseur peut décider en tout temps d'investir une fraction de son capital via la commande $u(t)$, où $0 \leq u(t) \leq 1$.
Cet investissement à un rendement constant $\gamma \in \R$.
Pour que l'investissement soit rentable, on suppose $\gamma >0$.
La croissance du capital est donc proportionnel à l'investissement réalisé $\dot{x}(t) = \gamma u(t) x(t)$.

Afin de maximiser le capital, on cherche à maximiser la possession de l'investisseur $(1-u(t))x(t)$, qui est la fraction du capital non investi.

Le problème se formule :
$$
\max_{x,u} \int_0^T (1-u(t))x(t) dt, \\
\dot{x}(t) = \gamma u(t) x(t), \quad \forall t \in [0,T]\\
 \quad 0 \leq u(t) \leq 1, \quad \forall t \in [0,T]\\
x(0)=x_0
$$

**En anglais:**

We aim to maximize an investor's capital over a time interval $x(t), t \in [0, T]$. The initial capital is $x(0) = x_0$. At any time, the investor can decide to invest a fraction of their capital using the command $u(t)$, where $0 \leq u(t) \leq 1$. This investment yields a constant return $\gamma \in \mathbb{R}$. For the investment to be profitable, we assume $\gamma > 0$. The growth of the capital is thus proportional to the investment made, given by $\dot{x}(t) = \gamma u(t) x(t)$.

To maximize the capital, we seek to maximize the investor's ownership $(1-u(t))x(t)$, which represents the fraction of the capital not invested.

The problem can be formulated as follows:

# Variante à plusieurs investissements
Dans cette variante, un investisseur a le choix entre plusieurs investissements.
Chacun des $n$ investissements possible est contrôlé par $u_i(t)$.
Chaque investissement à un rendement constant $\gamma_i$.
L'intérêt est de ne pas avoir uniquement des $\gamma_i$ positif.
La croissance du capital s'adapte $\dot{x}(t) = \sum_{i=1}^n \gamma_i u_i(t) x(t)$.

Le problème original est modifié tel que :
$$
\max_{x,u} \int_0^T (1-u(t))x(t) dt, \\
\dot{x}(t) = \sum_{i=1}^n \gamma_i u_i(t) x(t), \quad \forall t \in [0,T]\\
 \quad 0 \leq u_i(t) \leq 1, \quad \forall t \in [0,T], 1 \leq i \leq n\\
 \sum_{i=1}^n u_i(t) \leq 1, \quad \forall t \in [0,T]\\
x(0)=x_0
$$

**En anglais:**

In this variation, an investor has the choice between multiple investments. Each of the $n$ possible investments is controlled by $u_i(t)$. Each investment yields a constant return $\gamma_i$. It's important to note that not all $\gamma_i$ are necessarily positive. The growth of the capital adjusts accordingly to $\dot{x}(t) = \sum_{i=1}^n \gamma_i u_i(t) x(t)$.

The modified problem is formulated as follows:

# Variante à plusieurs investissements
Cette dernière variante permet d'intégrer les fluctuations réelles des rendements.
Ainsi, chaque investissement à un rendement constant $\gamma_i(t), t \in [0,T]$.
La croissance du capital est alors $\dot{x}(t) = \sum_{i=1}^n \gamma_i(t) u_i(t) x(t)$.

Ce dernier problème se formule :
$$
\max_{x,u} \int_0^T (1-u(t))x(t) dt, \\
\dot{x}(t) = \sum_{i=1}^n \gamma_i(t) u_i(t) x(t), \quad \forall t \in [0,T]\\
 \quad 0 \leq u_i(t) \leq 1, \quad \forall t \in [0,T], 1 \leq i \leq n\\
 \sum_{i=1}^n u_i(t) \leq 1, \quad \forall t \in [0,T]\\
x(0)=x_0
$$

**En anglais** :

This last variant allows for the incorporation of actual fluctuations in returns. Thus, each investment has a time-dependent constant return $\gamma_i(t), t \in [0,T]$. The growth of the capital adjusts accordingly to $\dot{x}(t) = \sum_{i=1}^n \gamma_i(t) u_i(t) x(t)$.

The formulation of this final problem is: