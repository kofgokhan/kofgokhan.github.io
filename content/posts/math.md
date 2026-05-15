+++
date = '2026-05-13T21:33:52+03:00'
draft = false
title = 'Math'
+++

# Bilevel Optimization
A bilevel optimization problem models the decision of a leader under the best response of the
follower and the follower's decisions in response to the leader decisions. A pure integer linear    bilevel optimization problem can be described as follows:

    \[
    \begin{align*}
    \min \ & (c^1)^\top x + (d^1)^\top y \\
    \text{s.t.} \ & A^1 x + B^1 y \le b^1, \\
    \ & G x \le g, \\
    \ & x \ge 0, \\
    \ & \begin{aligned} y \in \arg\min_{y'} \ & (d^2)^\top y' \\
    \text{s.t.} \ & A^2 x + B^2 y' \le b^2, \\
    \ & H y \ge h.
    \end{aligned}
    \end{align*}
    \]

    </span> where \(c^1 \in \mathbb{R}^{n_x}\), \(d^1 \in \mathbb{R}^{n_y}\), \(A^1 \in \mathbb{R}^{m_1
    \times n_x}\), \(B^1 \in \mathbb{R}^{m_1 \times n_y}\), \(b^1 \in \mathbb{R}^{m_1}\), \(G \in
    \mathbb{R}^{m_x \times n_x}\), \(g \in \mathbb{R}^{m_x}\), \(d^2 \in \mathbb{R}^{n_y}\), \(A^2 \in
    \mathbb{R}^{m_2 \times n_x}\), \(B^2 \in \mathbb{R}^{m_2 \times n_y}\), \(b^2 \in
    \mathbb{R}^{m_2}\), \(H \in \mathbb{R}^{m_y \times n_y}\), \(h \in \mathbb{R}^{m_y}\).

## Solution Methods
Lorem ipsum dolor sit amet consectetur adipisicing elit. Tenetur, mollitia. Modi saepe in
necessitatibus odit obcaecati, perspiciatis aliquid suscipit quae molestiae a est libero? Maxime 
fugiat consectetur architecto consequatur totam.
Lorem ipsum dolor sit amet consectetur adipisicing elit. Tenetur, mollitia. Modi saepe in
necessitatibus odit obcaecati, perspiciatis aliquid suscipit quae molestiae a est libero? Maxime 
fugiat consectetur architecto consequatur totam.
Lorem ipsum dolor sit amet consectetur adipisicing elit. Tenetur, mollitia. Modi saepe in
necessitatibus odit obcaecati, perspiciatis aliquid suscipit quae molestiae a est libero? Maxime 
fugiat consectetur architecto consequatur totam.
Lorem ipsum dolor sit amet consectetur adipisicing elit. Tenetur, mollitia. Modi saepe in
necessitatibus odit obcaecati, perspiciatis aliquid suscipit quae molestiae a est libero? Maxime 
fugiat consectetur architecto consequatur totam.
Lorem ipsum dolor sit amet consectetur adipisicing elit. Tenetur, mollitia. Modi saepe in
necessitatibus odit obcaecati, perspiciatis aliquid suscipit quae molestiae a est libero? Maxime 
fugiat consectetur architecto consequatur totam.
Lorem ipsum dolor sit amet consectetur adipisicing elit. Tenetur, mollitia. Modi saepe in
necessitatibus odit obcaecati, perspiciatis aliquid suscipit quae molestiae a est libero? Maxime 
fugiat consectetur architecto consequatur totam.
Lorem ipsum dolor sit amet consectetur adipisicing elit. Tenetur, mollitia. Modi saepe in
necessitatibus odit obcaecati, perspiciatis aliquid suscipit quae molestiae a est libero? Maxime 
fugiat consectetur architecto consequatur totam.