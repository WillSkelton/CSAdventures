# Chapter 25: Electric Potential

- [Chapter 25: Electric Potential](#chapter-25-electric-potential)
- [Chapter 25.1: Electric Potential Energy](#chapter-251-electric-potential-energy)
  - [Refresher on Energy and Work](#refresher-on-energy-and-work)
  - [Energy and Electricity](#energy-and-electricity)
  - [Uniform Electric Fields](#uniform-electric-fields)
    - [Work Done on a Charge by an Electric Field](#work-done-on-a-charge-by-an-electric-field)
    - [Work Done by the Electric Field Causes the Electric Potential Energy to Change By](#work-done-by-the-electric-field-causes-the-electric-potential-energy-to-change-by)
- [Chapter 25.2: Potential Energy of Point Charges](#chapter-252-potential-energy-of-point-charges)

# Chapter 25.1: Electric Potential Energy

So hopefully, you remember the concept of energy from the previous semester of physics. But if you don't or you're like me and your professor was a punk-ass who had a math degree from Devry "University", here's a refresher:

## Refresher on Energy and Work

Oxford Dictionary gives two definitions:

1. the strength and vitality required for sustained physical or mental activity.
2. power derived from the utilization of physical or chemical resources, especially to provide light and heat or to work machines.

You can think of energy in physics like you think of your own energy. For example, it costs me little to almost no energy to do something I enjoy like watching movies with my sister, sleeping, playing video games, or spending 4 hours making memes in MS Paint. However, Monday morning rolls around and I have to wake up at 6:00 and spend the first half of my day putting out fires at work and the second half trying to figure out what the flying fuck my physics professor wants me to decipher from his horrible lab instructions. That takes A LOT of mental energy. So really, there are two main things to remember about energy:

> 1. Energy is the unit of how hard it is to make something perform **work**
> 2. Energy can't be created or destroyed. Only transferred.

Now we have **Work**. Work is done when we move a thing from one place to another. Hopefully, you remember this equation:

$$
W = \vec{F}\cdot \Delta \vec{r} = F\ \Delta r\ cos(\theta)
$$

With $\Delta r$ being the displacement and $\theta$ being the angle between the two vectors.

What happens if our force isn't constant or parallel to our displacement? Well we thought of that and the answer is integrals which I know to be everyone's favorite.

$$
W = \int\limits^{x_f}_{x_i}{F(x)\cdot cos(\theta)\ dx}
$$

This looks spooky but really what it's doing is breaking up the forces and angles into little segments and adding them together. After all, **integration is just spicy summation**.

## Energy and Electricity

Now, we're going to look back to Gravity. In this case, the book sucks so bad that instead, I'm using this [YouTube](https://www.youtube.com/watch?v=xrQCPYsoBKk) video by user "Doc Schuster". I like this dude because he's the same kind of smart-ass that I am and his teaching strategy is how I learn.

Since we can't really touch electricity (or interact with it) like gravity, it's a little harder to wrap our brains around. But think back to gravity and potential energy. We had:

$$
\text{Force} \rightarrow \vec{F} = mg
$$

$$
\text{Energy} \rightarrow \vec{E} = mgh
$$

where $m$ is mass, $g$ is the force of gravity, and $h$ is height. Now, with gravity and potential energy, the higher you go up, or in other words, the more you resist gravity, the more it wants to pull you back down. Similarly, the closer you get to the ground you get, the calmer and less agitated gravity gets about you opposing its will. Thus, the potential energy is directly related to the distance you move into or away from the force.

The same goes for Electric Potential. The more you resist an electric field and move against it, the more electric potential you have.

## Uniform Electric Fields

![Figure 25.3](./assets/fig-2503.png)

This is a charged parallel plate capacitor with distance $d$ between the two plates. With gravity, we know that it always points down. However, with capacitors, they can point wherever. So we've oriented it such that the electric field points from positive to negative so that $\vec{E}$ points in the negative s direction the same way gravity points in the negative direction. Now that we're using $s$ which is the distance from the negative plate, we can flip this bad boy around however we want because concepts like "up" and "down" are irrelevant.

Now, let's pretend that we put a little particle in there. The positive side will push it towards the negative side and the negative charge will pull it to the negative side. This is where the conservation of energy comes into play. As this particle speeds up and moves towards the negative plate, it's distance against the negative plate decreases and with it decreases the electric potential energy. This is the same way a falling object looses gravitational potential energy as it falls. Gravitational and Electric fields don't like things resisting them and when those things stop resisting, Gravity and Electricity will put them where they want them.

In terms of formulas, the Conservation of Energy looks like this:

### Work Done on a Charge by an Electric Field

$$
W_{elec} = F \cdot \Delta r \cdot cos\theta \degree = qE\cdot |s_f-s_i| = \bigg[qEs_f-qEs_i\bigg]
$$

In this case, $\theta =0$ because the electric field in the capacitor is horizontal.

### Work Done by the Electric Field Causes the Electric Potential Energy to Change By

$$
\Delta U_{elec} = U_f-U_i = -W_{elec}(i\rightarrow f) = \bigg[qE_f-qE_i\bigg]
$$

$$
Or
$$

$$
U_{elec}=U_0+qEs
$$

Here's the main takeaway:
![Figure 25.3](./assets/fig-2504.png)

---

# Chapter 25.2: Potential Energy of Point Charges

The book gives a weird example where they tell you to imagine two charges and pretend that one is "glued down". In this context, I think it's dumb to try to imagine things you're not familiar with so instead I'm going to give an analogous example with magnets because we've all played with magnets before.

Let's say we have a magnet fixed to a table with its north pole facing to the left. We'll call this magnet $A$. Now, let's say we have another magnet $(B)$ that's to the left of magnet $A$ and has its north pole facing to the right. Now we have a setup where we can try to touch magnet $B$ to $A$ bus since their north poles are facing each other, they're going to try to stop you. Think about magnet $A$. As you get $B$ closer to it, they're pushing harder and harder against each other and the forces acting on each one by the other is increasing. Even though magnetic fields and electric fields are different, they're similar in this case. Now, we can switch back over to electric charges.

The main part of this section is to calculate the energy of the interaction which can be done by calculating the work done by moving the free charge towards or away from the fixed one. That is:

$$
W_{elec}=\int\limits_{x_i}^{x_f} F_{1\ on 2}\ dx
$$

Since we're just moving this along a table, we're only going in the x-direction and $cos\ \theta = 1$. Thus:

$$
W_{elec}=\int\limits_{x_i}^{x_f}\frac{Kq_1q_2}{x^2}\ dx = \Bigg[Kq_1q_2\frac{-1}{x}\Bigg]\Bigg |_{x_i}^{x_f} = -\frac{Kq_1q_2}{x_f} + \frac{Kq_1q_2}{x_i}
$$

Then, to get potential energy, we get the difference in energy which is:

$$
\Delta U_{elec} = U_f-U_i = -W_{elec}(i\rightarrow f) = \frac{Kq_1q_2}{x_f} - \frac{Kq_1q_2}{x_i}
$$

$\Delta U_{elec} = -W_{elec}(i\rightarrow f)$ because the work to go from $i$ to $f$ is $-1 \cdot(\text{the work to go from } f \text{ to } i)$ If all that is blowing your mind, don't worry about it because we can simplify it down to:

$$
U_{elec} = \frac{Kq_1q_2}{x}
$$

How's that for simplification?

We're not done though. What if we have more than two charges? Don't even trip. We have a formula for that too:

$$
U_{elec} = \sum \limits_{i<j} \frac{Kq_iq_j}{r_{ij}}
$$

In order to find the potential energy of multiple charges, all we have to do is sum up all the potential energies of each pair. So if we had three charges, we'd find the energies of 1 on 2, 2 on 3, and 3 on 1.

---