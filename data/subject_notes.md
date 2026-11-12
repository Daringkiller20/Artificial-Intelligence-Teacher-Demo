PHYSICAL REVIEW X 6, 041052 (2016)
Quantum Trajectories and Their Statistics for Remotely Entangled Quantum Bits
Areeya Chantasri,1,2 Mollie E. Kimchi-Schwartz,3 Nicolas Roch,4 Irfan Siddiqi,3 and Andrew N. Jordan1,2,5
1Department of Physics and Astronomy, University of Rochester, Rochester, New York 14627, USA
2Center for Coherence and Quantum Optics, University of Rochester, Rochester, New York 14627, USA
3Quantum Nanoelectronics Laboratory, Department of Physics,
University of California, Berkeley, California 94720, USA
4Université Grenoble Alpes, Institut NEEL, F-38000 Grenoble, France
and CNRS, Institut NEEL, F-38000 Grenoble, France
5Institute for Quantum Studies, Chapman University, 1 University Drive, Orange, California 92866, USA
(Received 31 March 2016; revised manuscript received 6 October 2016; published 14 December 2016)
We experimentally and theoretically investigate the quantum trajectories of jointly monitored transmon
qubits embedded in spatially separated microwave cavities. Using nearly quantum-noise-limited super
conducting amplifiers and an optimized setup to reduce signal loss between cavities, we can efficiently
track measurement-induced entanglement generation as a continuous process for single realizations of the
experiment. The quantum trajectories of transmon qubits naturally split into low and high entanglement
classes. The distribution of concurrence is found at any given time, and we explore the dynamics of
entanglement creation in the state space. The distribution exhibits a sharp cutoff in the high concurrence
limit, defining a maximal concurrence boundary. The most-likely paths of the qubits’ trajectories are also
investigated, resulting in three probable paths, gradually projecting the system to two even subspaces and
an odd subspace, conforming to a “half-parity” measurement. We also investigate the most-likely time for
the individual trajectories to reach their most entangled state, and we find that there are two solutions for the
local maximum, corresponding to the low and high entanglement routes. The theoretical predictions show
excellent agreement with the experimental entangled-qubit trajectory data.
DOI: 10.1103/PhysRevX.6.041052
I. INTRODUCTION
Measurement-induced entanglement of spatially sepa
rated quantum systems is a startling prediction of quantum
mechanics [1–7]. Recent experiments have demonstrated
this effect via single-photon heralding [8–11], as well as via
continuous measurement of photons interacting with qubits
[12]. The latter has the advantage of being able to
investigate the physics of entanglement creation continu
ously, leading to new effects such as the sudden creation of
entanglement after a finite measurement period, dubbed
entanglement genesis [6]. However, many questions are
outstanding, such as the following: (a) What is the complete
characterization of the dynamics of entanglement creation
as a continuous trajectory? (b) What is the statistical
distribution of the entanglement at any time during the
process? (c) What is the most-likely way entanglement is
generated? In this work, we give a systematic answer to
these questions, as well as others, by analyzing experi
mentally entangled quantum trajectories of jointly mea
sured transmon qubits and showing excellent agreement
with the theory developed here.
Published by the American Physical Society under the terms of
the Creative Commons Attribution 3.0 License. Further distri
bution of this work must maintain attribution to the author(s) and
the published article’s title, journal citation, and DOI.
2160-3308=16=6(4)=041052(14)
Subject Areas: Quantum Physics, Quantum Information
The rapid development of quantum information science
in the superconducting domain [13] has seen an exponen
tial increase in qubit coherence time within the past decade,
leading to many scientific advances [14]. This technologi
cal progress has led to a wide variety of advances in
quantum physics, as observed and controlled in these
systems, including greater than 99% fidelity in single-qubit
quantum gates [15], multiqubit-entanglement-generating
gates [16], the violation of Bell’s inequality [17], and
quantum-process tomography [18]. Recent developments
include the observation of quantum states of light in
resonators [19], as well as nearly quantum-limited para
metric amplifiers [20,21].
The improvement of coherent quantum hardware has
brought with it a renewed focus on the physics of quantum
measurement. Generalized measurements have been car
ried out in superconducting qubits [22], realizing probabi
listic measurement reversal [23,24], weak values [25,26],
and their connection with generalized Leggett-Garg
inequalities [27]. Continuous measurements [28] in super
conducting systems have only recently been realized,
owing to the challenge associated with high-fidelity detec
tion of microwave signals near the single-photon level. In
particular, experimental achievements include continuous
feedback control [29,30] and the tracking of trajectories in
individual experiments in the plain measurement case
[31–34] as well as with a concurrent Rabi drive [35].
041052-1
Published by the American Physical Society
AREEYA CHANTASRI et al.
PHYS. REV. X 6, 041052 (2016)
These experiments show detailed quantitative agreement
with theory, indicating a good understanding of quantities
such as the most-likely path of the quantum state between
boundary conditions, predicted with an action principle of
an associated stochastic path integral [36–38].
Going beyond a single qubit opens the possibility of
measurement-induced entanglement, using a dissipative
process as a tool to generate quantum correlations. For
quantum architectures building upon transitions at optical
frequencies [8–11], this feat has typically been achieved by
relying on the correlated detection of photons at the output
of a beam splitter [1] to herald an entangled state. While
powerful, this measurement protocol is binary and instan
taneous, and it allows no insight into the dynamical
processes underlying the generation of the entangled state.
In solid-state systems, such as superconducting qubit
transitions in the microwave regime, there has been
tremendous interest in continuously generating bipartite
[3–6,39] and multipartite [2,40,41] entangled states, using
weak measurements that slowly interact with the qubits, in
such a way that enables the resolution of the dynamical
aspects of the entangling backaction. Analog feedback
control can naturally be applied in the weak continuous
measurement regimes [42–44], and digital feedback
generated entanglement has already been demonstrated
[45]. Joint measurement is uniquely useful as a means to
generate entanglement between remote qubits [12,46–50],
for which no local coupling exists and therefore no unitary
means of generating entanglement are available.
The chief advantage of the continuous approach is in the
efficiency of entanglementgeneration.Incontrasttophoton
counting schemes (in which entanglement-generation rates
are heavily limited by photon losses), continuous measure
ment enables an entanglement-generation rate limited only
by the premeasurement initial state and the postselection
criterion, which are both experimental choices. However,
continuous measurements may be highly sensitive to dis
sipative losses and inefficiencies in amplification.
Understandingandstudyingthedynamicalprocessesunder
lying continuous measurement-induced entanglement is
therefore critical for balancing these tradeoffs.
In this work, we combine an efficient quantum amplifier
with a continuous half-parity measurement to conduct
detailed experimental and theoretical investigations of
the statistics of individual trajectories of qubit pairs as
they undergo the entangling process. The half-parity
measurement can distinguish between the even-parity
and odd-parity subspaces, similar to a full-parity measure
ment, but also between the two states j00i and j11i in the
even-parity subspace, leaving the odd subspace entangled.
By peering into the ensemble, we can understand the
full spectrum of evolution paths as the two-qubit state
gradually projects onto the entangled subspace or onto a
trivial separable state. We explore the probability distribu
tion of the qubits’ concurrence to understand how the
distribution changes in time, from a separable state with
zero concurrence, to projected states in either a separable
subspace or an entangled subspace. This can also be seen
from the most-likely path analysis, showing the emergence
of different most probable paths for each final state.
Moreover, we investigate the distribution of the time to
maximum concurrence, finding that the most probable time
to maximum values of concurrence has a bimodal structure.
Studying the statistics of a large set of trajectories—rather
than averaging over all of them to study the dynamics of the
ensemble—enables an unprecedented understanding of the
dynamics of entanglement creation under measurement.
The paper is organized as follows. In Sec. II, we describe
our transmon qubit measurement setup and the method of
reconstructing the joint trajectories. In Sec. III, we derive
the concurrence-readout relation and compute the distri
bution of concurrence as the measurement backaction
proceeds. This distribution is then compared with the data
generated from the experiment. In Sec. IV, we turn to the
most-likely path analysis, finding three possible paths that
the joint system takes from a separable initial state to final
entangled or separable states. The experimental most-likely
paths are generated independently to compare with the
theoretical prediction. We also discuss the distribution of
the time for the two qubits to reach their maximum
entanglement. The conclusions are presented in Sec. V.
Additional details of the most-likely path calculations and a
discussion of the parity meter are presented in the
appendixes.
II. TRAJECTORIES OF TRANSMON QUBITS
We consider a two-qubit system realized by super
conducting transmon qubits embedded in spatially sepa
rated microwave cavities in a setup optimized to reduce
losses between the cavities. These qubits are jointly
measured via a dispersive readout in a bounce-bounce
geometry [see Fig. 1(a)] in which a microwave tone is
sequentially reflected off of two copper cavities, each
containing a transmon qubit, and subsequently amplified
and measured via homodyne detection. The cavities are
directly joined by a circulator that enforces the unidirec
tional transfer of the coherent state. A single transmon
interacts with the light in its cavity via a dispersive
interaction of the form
Hj ¼χjσðjÞ
z a†a;
ð1Þ
where χj is the dispersive interaction strength of the light
interacting with the dipole moment of qubit j (cross-Kerr
nonlinearity between the qubit and the cavity), coupling to
its σðjÞ
z
Pauli observable. The net effect of the bounce
bounce geometry is that the effective interaction of the
combined system is described by a Hamiltonian of the form
H1 þH2.Afteramplification and homodynemeasurement,
041052-2
QUANTUM TRAJECTORIES AND THEIR STATISTICS FOR …
PHYS. REV. X 6, 041052 (2016)
(a)
(c)
(b)
(d)
FIG. 1. Experimental setup and transmon qubit trajectories. Panel (a) shows a simplified illustration of the experimental setup. Two
transmon qubits in two remote cavities are linked via a single microwave circulator in a bounce-bounce geometry; the output of the
circulator is routed to a high-efficiency amplification chain (not shown). The upper inset represents the distribution of the microwave
field in the (X1, X2) quadrature plane at the output of the amplifier. The three possible outcomes correspond to three different subspaces:
j00i, j11i, and the odd-parity subspace (spanned by the j01i and j10i states). Panel (b) shows the evolution in time of the measurement
outcome probability distribution pðVtÞ. Panel (c) shows the agreement between the experimentally generated conditional tomography
xiðVtÞ (symbols and shaded error bars) and the theoretical Bayesian reconstruction (dashed lines), for a single time t ¼ 0.48 μs. In panel
(d), we use such reconstructions to predict and verify the trajectory of a single iteration of the experiment, showing both density matrix
elements xi and concurrence (inset).
this interaction gives a dispersive phase shift of ϕ for
states j0i, j1i. The shift ϕ is given, in general, by
ϕj ¼ arg½αj0i;j − arg½αj1i;j , where αi;j represents the intra
cavity coherent state conditioned on state i of qubit j. In the
fully symmetric, weak measurement case (when all qubit
and cavity parameters are identical and χj¼1;2 ≪ κ), this
phase shift is given by ϕj ≈ 2χj=κj, where κj is the cavity
damping rate of cavity j.
In the bounce-bounce geometry, there generally exists a
probe frequency at which the dispersive shifts from both
transmon qubits are the same (ϕ1 ¼ ϕ2 ¼ φ), such that the
measurement tone can acquire a phase shift of either 2φ,0,
0, −2φ for states j00i, j01i, j10i, j11i. For small χ=κ,
this results in a half-parity measurement on the two qubits,
where the measurement result can distinguish between
three subspaces: the j00i state, the j11i state, and the odd
parity subspace, but not within the odd-parity subspace,
spanned by the j01i and j10i states. Conditioning on the
measurement results with a zero phase shift can lead to
creation of an entangled state within the odd-parity sub
space (superpositions of j01i and j10i).
When the output of the second cavity [on the right in
Fig. 1(a)] is directed to a nearly quantum-limited ampli
fication chain, the instantaneous homodyne detection
signal can be correlated with the measurement backaction
on the qubits; therefore, it can be used to track the evolution
of the system in time. By reducing the amplitude of the
coherent state used to measure the system, we can engineer
an entangling measurement with a characteristic measure
ment time ranging from several hundred nanoseconds to
several microseconds: Critically, these time scales are
easily resolvable experimentally. The dynamics or the
trajectory of the system state can be obtained via the full
master equations [46,47], using a two-cavity polaron
transformation to account for the cavity degree of freedom,
giving the stochastic master equation for the qubit trajec
tories. Alternatively, in a limit of large cavity decay rate
κ ≫jχj,thequbitevolution can be continuously tracked via
the quantum Bayesian approach [2,3], inferring the current
states of the system from the measurement readouts and
how likely they are to occur. The two approaches both show
good agreement in tracking the qubit pair state [12].
In this paper, we focus on the quantum Bayesian
approach, as it is directly related to the probability
distribution of the measurement readout and naturally leads
to the probability distribution of quantum trajectories. Let
us denote pðVtjiÞ as a probability density function of a
measurement readout Vt conditioned on the two-qubit
states i, where i ¼ 1, 2, 3, 4 represent the states j00i,
j01i, j10i, j11i, respectively. The quantum Bayesian update
041052-3
AREEYA CHANTASRI et al.
PHYS. REV. X 6, 041052 (2016)
for this type of double-qubit measurement provides a
convenient way to calculate the joint state at time t,given
a known state at the initial time and the readout Vt,
p
ρijð0Þ ffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffi
P4
pðVtjiÞpðVtjjÞ
e−γijt
ρijðtÞ¼
k¼1 ρkkð0ÞpðVtjkÞ
;
ð2Þ
where ρij denotes the ij element of the two-qubit density
matrix and γij is a decoherence rate associated with the
matrix element. The quantum Bayesian approach is equiv
alent to the positive-operator valued measure (POVM)
formalism [51], provided we identify the measurement
operators. In the case of no additional Rabi drives on either
qubit, the measurement operators are given by
p
MVt 
¼ 
ffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffi
pðVtjoddÞ
p
þ 
ffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffi
pðVtj1Þ
ðj01ih01jþj10ih10jÞ
p
j00ih00jþ 
ffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffi
pðVtj4Þ
j11ih11j;
ð3Þ
where the distribution pðVtjoddÞ¼pðVtj2Þ¼pðVtj3Þ is
the same for any state within the odd subspace. The
POVM elements, M†
Vt
MVt
, correctly integrate to the iden
tity operator in the two-qubit Hilbert space, understanding
that we integrate with a measure for Vt. Applying the state
update rule, conditioned on an observation of the readout
Vt, ρðtÞ¼MVt
ρð0ÞM†
Vt
=Tr½MVt
ρð0ÞM†
Vt
recovers Eq. (2)
in the case of no extra decoherence γij ¼ 0.
We define the readout Vt ≡ðf=tÞR t
0 
~ Vðt0Þdt0 − v0 as a
time average of a raw homodyne voltage signal rescaled
with a weight factor f and an offset v0, where f is chosen so
that the variance σ2
Vt 
¼ 1=4ηmt is a function of a quantum
efficiency of the homodyne measurement, ηm ≈ 0.22. The
total probability distribution
X4
pðVtÞ¼
k¼1
ρkkð0ÞpðVtjkÞ;
ð4Þ
shown in Fig. 1(b), slowly resolves into the three peaks
expected for a half-parity measurement.
The conditional readout distributions are well ap
proximated by Gaussian functions, giving pðVtjiÞ¼
ðt=πsÞ1=2 expf−ðVt − δviÞ2t=sg with the centering signals
δvi ¼ vi −v0 for i ¼ 1;…;4, where s ¼ 1=2ηm. The
measurement process cannot distinguish the two states
in the odd-parity subspace; therefore, the readout distribu
tions corresponding to the states j01i and j10i are com
pletely (or nearly) overlapped, giving δv2 ≈ δv3 ≈ 0 and
−δv1 ≈δv4 ≈δv. The measurement strength is character
ized by an inverse of a characteristic measurement time
τm ≈1=δv2ηm. The dephasing rates γij for δvi ≠ δvj are
dominated by the effect of the distinguishability between
states i and j, γij ∼ ðη−1
m −1Þðδvi −δvjÞ2=4s [2], resulting
in the strong suppression of all off-diagonal elements
except ρ23. In an ideal half-parity measurement, the decay
of ρ23 would be limited only by the intrinsic lifetimes of the
qubits; however, we must additionally account for exper
imental imperfections in the matching of δv2 and δv3 and
for the loss of photons between the two cavities. These
effects are included in the (slightly time-dependent)
dephasing rate γ23.
Since we expect most of the off-diagonal terms to damp
quickly, we only consider five relevant density matrix
elements: x1 ≡ ρ11, x2 ≡ ρ22, x3 ¼ ρ33, x4 ≡ ρ44, and x5 ≡
jρ23j [52]. In order to compare the Bayesian prediction to
the true density matrix, we perform conditional tomogra
phy [12,53] to experimentally reconstruct the full exper
imental mapping Vt ↦ρðVt;tÞ. In conditional tomography,
we collect an ensemble of trajectories that reach a particular
Vt at time t, and tomographically reconstruct that ensem
ble. This provides a density matrix conditioned on Vt. In
Fig. 1(c), we show good agreement between the Bayesian
prediction and conditional tomography reconstruction of
xiðVtÞ for a single measurement time t ¼ 0.48 μs. We show
examples of transmon qubit trajectories in Fig. 1(d) for an
initial state prepared in a product of ˆx states, i.e., the equal
superposition state ð1=2Þðj00iþj01iþj10iþj11iÞ, such
that the five relevant density matrix elements are
x0
1 ¼ x0
2 ¼ x0
3 ¼ x0
4 ¼ x0
5 ¼ 1=4. We show both the
Bayesian reconstruction and the tomographic verification,
which are in good agreement. This verifies that the
Bayesian reconstruction can be used to faithfully translate
a noisy measurement signal into the stochastic evolution of
a joint quantum state.
We conclude this section with a qualitative discussion
of the mechanisms behind the entanglement dynamics,
which will be followed up with a quantitative analysis in
the next section. As discussed previously, the half-parity
measurement can distinguish between the two even
parity states but not within the odd-parity subspace.
We can think of this measurement as a continuous version
of an ideal projective measurement with three projectors
Π1 ¼j00ih00j;Πodd ¼j01ih01jþj10ih10j;Π3 ¼j11ih11j,
which partition unity in the two-qubit-state space. Given an
arbitrary separable pure state, jψi¼ða1j0i1 þ b1j1i1Þ×
ða2j0i2 þ b2j1i2Þ, textbook wave-function collapse upon
measurement of the odd result gives the (un-normalized)
state j ~ψi¼a1b2j01iþb1a2j10i. Clearly, for certain val
ues of a1, b1, a2, b2, the postcollapse state will be
entangled. In particular, the choice a1 ¼ b1 ¼ a2 ¼ b2 ¼
1= ffiffiffi 2
p previously mentioned will result in a maximally
entangled state. Mathematically, entanglement is created
because the odd projection operator cannot distinguish
within the odd subspace.
Of the three possibilities between collapse to the two
even states or to the odd subspace, quantum mechanics
only tells us the statistics of these events happening; it does
not predict which will occur in a given run. In addition, in
the continuous measurement case, we can only predict the
041052-4
QUANTUM TRAJECTORIES AND THEIR STATISTICS FOR …
PHYS. REV. X 6, 041052 (2016)
statistics of the system by choosing one eventual path
among the various choices. However, because the proba
bility distribution of the results is of the simple form (4),we
may understand the gradual transition from separable to
entangled as a given measurement result indicating which
basis state the system is collapsing into, masked by additive
quantum noise. Transitions from one branch to another can
occur and may be understood as originating from the tails
of the distributions overlapping. As time develops, those
tails decrease, so a larger (and less likely) quantum
fluctuation is required in order to cause the quantum
system to transition from one branch to another. This
increase of knowledge resulting in an altered quantum state
may be understood as Bayesian inference, suitably gener
alized to take quantum entanglement into account, Eq. (2).
III. CONCURRENCE TRAJECTORIES AND
THEIR DISTRIBUTION
We now give a quantitative analysis of the statistical
process of entanglement creation for continuous measure
ment. As a measure of entanglement between two parties
such as the transmon qubits, concurrence is a convenient
choice and can be computed directly from the density
matrix of the system [54]. The concurrence formula for
the half-parity setup is greatly simplified because of
the suppression of most matrix elements, resulting in an
X-shape density matrix, of which the concurrence is
calculated from [54,55]
p
CðtÞ¼2maxf0;x5ðtÞ − 
ffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffi
x1ðtÞx4ðtÞ
g:
ð5Þ
The value of concurrence ranges from 0 for a separable
state to 1 for the Bell states. The concurrence trajectory of
an exemplar trajectory is shown in the inset to Fig. 1(d).In
this section, we use the simplified formula Eq. (5) to show
that the concurrence of the two-qubit state can be deter
mined directly from the measurement readout, which then
leads to the derivation of the concurrence probability
distribution as a function of the measurement readout
and measuring time.
A. Concurrence-readout relationship
Let us consider the concurrence formula in Eq. (5),
where its value is determined by the second term in the
brackets, which we denote ct ≡ 2fx5ðtÞ − ffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffi
p
x1ðtÞx4ðtÞ
g.If
ct is a non-negative quantity (i.e., ct ≥ 0), then the
concurrence is simply given by CðtÞ¼ct. At the end of
this section, we show that this is always the case for our
chosen initial qubit state and parameter regimes, but it is not
true in general [6]. From the Bayesian update in Eq. (2),we
calculate the quantity
ct ¼2
N
n
x0
5 
ffiffiffiffiffiffiffiffiffiffiffi
P2P3
q
p 
e−γt− 
ffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffi
x0
1x0
4P1P4
o
;
ð6Þ
where x0
i for i ¼ 1;…;5 are the matrix elements of the
initial qubit state, and γ ¼ γ23. We have used simplified
notations Pi ≡ pðVtjiÞ for the probability distributions, and
N for a normalized factor given by N ¼ P4
k¼1xkð0ÞPk.
Substituting the probability distribution functions with
the Gaussian functions of the means δvi for i ¼ 1;…;4,we
obtain a form of ct explicitly as a function of Vt and t,
2
ctðVt;tÞ¼
M
q
ffiffiffiffiffiffiffiffiffi
fx0
5eðα23Vt−β23−γÞt −
x0
1x0
4
eðα14Vt−β14Þtg;
ð7Þ
where the prefactor is given by M ¼ P4
i¼1x0
ie2αiVtt−2βit
using a set of defined variables: αi ¼ δvi=s, αij ¼ αi þ αj,
βi ¼ δv2
i=2s, βij ¼ βi þ βj, and s ¼ 1=2ηm.
The quantity ct in Eq. (7) would represent the actual
concurrence of the qubit state at any time t, ifcðtÞ ≥ 0 is
satisfied. For our chosen initial state, a product of single
qubit ˆx states, x0
1 ¼ x0
2 ¼ x0
3 ¼ x0
4 ¼ x0
5 ¼ 1=4, the quantity
ct is non-negative whenever the condition ðγ − α23Vt þ
β23Þ < ðβ14 −α14VtÞ is true. From the experimental data
(e.g., for the setup with τm ¼ 0.60 μs), we have −δv1 ≈ δv4
and δv2 ≈δv3 ≈0 (giving α14, α23, β23 ≈0) and
β14 ∼ 3.2 MHz, while γ < 0.6 MHz. Therefore, the con
dition is always satisfied, and the second term in the
brackets of Eq. (7) decays faster than the first term,
resulting in a quantity that is always non-negative.
Consequently, the quantity in Eq. (7) gives the concur
rence-readout relationship CðVt;tÞ¼ctðVt;tÞ, and the
concurrence at any time t can be determined directly from
the time-averaged measurement readout Vt.
The concurrence formula in Eq. (7) can be simplified
further by considering a perfectly symmetric half-parity
measurement, δv2 ¼ δv3 ¼ 0and−δv1 ¼ δv4 ¼ δv.Given
the initial state, a product of two qubit ˆx states, the
concurrence is then given by
Cps;ˆxðVt;tÞ¼
e−γt − e−δv2t=s
1 þcoshð2Vtδvt=sÞe−δv2t=s 
;
ð8Þ
where the subscript “ps, ˆx” indicates the perfectly
symmetric half-parity measurement given the specific
initial state.
B. Probability density function for
concurrence trajectories
From the direct relationship between the measurement
readout and the concurrence of the qubit state, the prob
ability density function of the concurrence can be derived
from the probability distribution of the time-averaged
signal Vt. The distribution of the time-averaged readout
is given by
041052-5
AREEYA CHANTASRI et al.
x0
ipðVtjiÞ:
ð9Þ
PHYS. REV. X 6, 041052 (2016)
X4
pðVtÞ¼
i¼1
The variance of the distribution σ2
Vt 
¼ s=2t narrows as time
increases, leading to the collapse of the joint qubit state into
three categories: j00i state, j11i state, and some super
position state of j01i and j10i after a few characteristic
measurement times τm.
Knowing the probability density function of the time
averaged signal, we follow the transformation of random
variables Vt → C using the concurrence-readout relation
ship, Eq. (7) [or Eq. (8) for a perfectly symmetric case]. The
concurrence CðVt;tÞ is not a monotonic function in Vt;
instead, it has a bell-like shape, as shown in the inset of
Fig. 2(a). We write the cumulative distribution function of
the concurrence FC;tðcÞ¼pC;tðC ≤ cÞ¼pðVt ≤ V−Þþ
f1 −pðVt ≤ VþÞg, where pC;tðcÞ is a probability density
function for the concurrence, and Vþ, V− are two solutions
that arise from solving Eq. (7) [or Eq. (8)], CðVt;tÞ¼c.
The concurrence distribution is then obtained by taking a
derivative of the cumulative distribution,
pC;tðcÞ¼pðV−Þ
∂V−
∂c þpðVþÞ
noting that V−ðc;tÞ and Vþðc;tÞ are functions of the
concurrence c and time t. The full solution of pC;tðcÞ is
quite lengthy and is not shown.
We showinFig. 2(a) the plots of concurrence probability
distributions (10) for different values of time t, and in
Figs. 2(b) and 2(c) the density plot comparing the theory
and the transmon experiment. At an early time, the
distribution of concurrence is narrowly peaked near its
maximum, which increases over time, whereas at later
times, a second peak emerges near the zero concurrence,
showing a bimodal distribution. In Fig. 2(b), the theoretical
histogram for the concurrence is obtained by integrating the
theory curves, Eq. (10), for the probability over small
intervals δc ≈ 0.015. This integration makes a fair com
parison with the histogram of the experimental data in
Fig. 2(c), calculated with a bin size of 0.015. We note that a
short delay in the experimental entanglement creation is a
result of the cavity ring-up time, which will be discussed
more in the next section.
We stress that the concurrence distribution has a sharp
upper bound [shown as a grey dotted curve in Fig. 2(a)],
which the concurrence cannot exceed. In order to under
stand why the probability distribution for the concurrence
has a sharp upper cutoff at any time, we recall that the
density matrix of the two-qubit system, conditioned on the
time-integrated readout Vt, is entirely specified by that
(random) outcome, together with the initial state, the
dephasing rate, and other parameters of the problem,
Eq. (2). Consequently, the concurrence is controlled by
Vt, as in Eq. (8). As can be seen from the inset of Fig. 2(a),
(a)
(b)
(c)
∂Vþ
∂c ; ð10Þ
FIG. 2. Concurrence distribution for the qubits under the half
parity measurement. In panel (a) we plot the concurrence
probability density function, Eq. (10), for different values of
time. The values of time for the presented curves are chosen so as
to see their unique features as they develop. The grey dotted curve
joining the high-concurrence peaks shows the concurrence upper
bound, Eq. (11). The inset shows an example of how the
concurrence (at time t ¼ 1 μs) varies as a function of the readout
Vt. Panels (b) and (c) are the histograms of the concurrence at any
time points from t ¼ 0 to T ¼ 1.6 μs (with a step size 0.01 μs),
comparing theory and experimental data. For the theory plot, we
coarse-grain the distribution pC;tðcÞ in Eq. (10) by integrating it
with a pixel size δc∼0.015, which is the bin size of the
experimental histogram. For presentation purposes, a histogram
at any time t is normalized by its maximum element.
the concurrence, plotted as a function of the measured
signal Vt, is bounded from above for any fixed time t by
some amount we call Cmax, and consequently, any value of
concurrence higher than that maximum (whose value will
change as the time increases) cannot be realized. Therefore,
the probability distribution of concurrence has a sharp
upper cutoff given by CmaxðtÞ. Physically, this indicates that
there is an upper limit on how fast entanglement can be
created by the continuous measurement in this situation,
even for rare events of the measurement process.
041052-6
QUANTUM TRAJECTORIES AND THEIR STATISTICS FOR …
PHYS. REV. X 6, 041052 (2016)
For the perfectly symmetric case in Eq. (8), we find an
analytic solution for the upper bound of the concurrence,
knowing that coshðxÞ has its minimum at x ¼ 0 and
Cps;ˆxðVtÞ has its maximum at Vt ¼ 0; consequently, the
concurrence upper bound is given by
Cmax;ps;ˆxðtÞ¼
e−γt − e−δv2t=s
1 þe−δv2t=s 
:
ð11Þ
The behavior of this bound is a result of two competing
rates—the extra dephasing rate γ and a measurement rate
δv2=s. Equation (11) increases from zero for small times
and decays for a long time after reaching its maximum
concurrence, as seen in Fig. 2. The maximum possible
concurrence for this qubit half-parity measurement and the
time this happens can be obtained from this relation. More
about the time to reach maximum concurrence will be
discussed in Sec. IV C.
IV. MOST-LIKELY PATH ANALYSIS
In addition to the distribution analysis in the previous
section, where we treated the concurrence at each point in
time independent from any other times, we now incorporate
the notion of connected trajectories, finding a probability
density function for quantum trajectories and their most
likely paths. These most-likely paths describe routes with
the highest probability density, taking into account that all
of the points in the trajectory ensemble are connected via
quantum-state update rules, e.g., in Eq. (2).Aswehave
seen previously, the concurrence distribution exhibits a
transition from a single-peak distribution to double-peak
distributions, one at the upper bound concurrence and
another near zero concurrence. Here, with the notion of
trajectories, we also see that the two-qubit state starting in
its initial state gradually collapses to three subspaces: the
j00i subspace, the j11i subspace, and the odd subspace, as
described by three most-likely routes.
Let us consider the five nontrivial elements of the two
qubit density matrix fx1;x2;x3;x4;x5g and treat each
element as an independent variable. Each state trajectory
is represented by a time series of these five elements, which
corresponds to one realization of the measurement readout
~
fvtg¼fv0;vδt;v2δt;…;vtg, where we define vt ¼
ðf=δtÞR tþδt
t
Vðt0Þdt0 − v0 as an instantaneous readout at
time t with an integration time δt. Since the readout vt’s are
assumed to be Markovian and only depend on the qubit
states right before the measurement, a joint probability
density function for the readout realization is given by
Y t
PðfvtgÞ ¼
t0¼0
X4
k¼1
xk;t0pðvt0 jkÞ ;
ð12Þ
a product of probability distributions of vt0 from t0 ¼ 0 to
t0 ¼ t with a time step δt. The probability density function
ffiffiffiffiffiffiffiffiffiffiffi
for an instantaneous readout is given by pðvtjiÞ¼
δt=πs
p expf−ðvt−δviÞ2δt=sg for i ¼ 1,2,3,4.
To derive the most-likely path for these two-qubit
trajectories, we use the Bayesian update equation for the
two-qubit state Eq. (2), adapted to a state update every time
step δt, and then we maximize the joint probability density
Eq. (12), constraining the state update equations. Following
the most-likely path analysis for quantum states under
continuous measurement [36,37] and introducing Lagrange
multipliers fp1;p2;p3;p4;p5g for the constraints, we
obtain differential equations for an optimal path in the
qubit-state space,
∂txi ¼þxi
s
X
4
k¼1
xkf2vtðδvi − δvkÞ − δv2
i þ δv2
kg;
∂tx5 ¼ −γx5 þx5
s vtðδv2 þδv3Þ−
X4
þ
k¼1
xkðδv2
k − 2vtδvkÞ ;
ðδv2
2 þ δv3
3Þ
2
ð13aÞ
ð13bÞ
where i ¼ 1;…;4 for the first line and the variables xk are
time-dependent functions. We note that vt in these equa
tions behaves as a “smooth” optimal readout, which is a
function of the qubit density matrices and their Lagrange
multipliers, determining an optimal path from an initial
state to its final state [36]. An optimal path is a solution of
ten differential equations: five for the qubit-state variables,
Eq. (13), another five for Lagrange multipliers, and the
optimal readout as a function of both sets of variables (see
Appendix A). These equations describe most-likely paths
for a measurement with any values of δv1;…;4 and can also
be generalized to include the effect of external drives on the
two-qubit state. However, in the absence of an external
drive, these can be simplified, as we will see in the next
section.
A. Most-likely paths for joint measurement
of transmon qubits
In this work, where the transmon qubits only evolve with
the influence of the measurement backaction, the optimal
readout is found to be constant in time (see Appendix A).
We can therefore bypass solving the full set of differential
equations [49] and only compute the qubit evolution in
Eq. (13) with constant vt, looking for measurement results
with maximum likelihood density. To estimate the like
lihood density of a two-qubit trajectory, we evaluate a
logarithm of the probability density function Eq. (12)
approximated to first order in δt [36] to obtain
Z t
logPðfvtgÞ ≈ S0 −
0
4
ðvt0 − δvkÞ2xk;t0 ; ð14Þ
dt0 1
s
X
k¼1
041052-7
AREEYA CHANTASRI et al.
Da;b ¼ δt
X t
Tr
;
PHYS. REV. X 6, 041052 (2016)
where S0 represents a state-independent part of the joint
probability density function P. We show in the insets of
Figs. 3(a)–3(c) examples of the approximated log
likelihood density as functions of optimal readout vt, for
three different measurement strengths. In the case of
τm ≈2.10 μs, there is only one maximum likelihood value
located at vt ≈ δv2;3, which gives the most-likely path with
high concurrence, shown as a solid curve in Fig. 3(a);
whereas, in the stronger measurement cases, Figs. 3(b)
and (c), the approximated log-likelihood density has three
local maxima: the middle ones, vt ≈ δv2;3, corresponding to
most-likely paths collapsed to entangled states (high-con
currence branches); and the sided peaks, vt ≈ δv1 and
vt ≈δv4, corresponding to two branches of most-likely
paths collapsed to j00i and j11i states (low-concurrence
branches), respectively. We note that this technique of
finding multiple most-likely paths is not under final-state
constraints as in Refs. [35,36].
We choose to compare the theoretical most-likely paths
with high-trajectory density paths extracted from the
experimental data, using the trace distance method. We
collect an ensemble of 104 transmon trajectories and then
compute average trace distances between any two trajec
tories (e.g., ρa and ρb),
(a)
(b)
q
2T
ffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffiffi
ðρaðt0Þ − ρbðt0ÞÞ†ðρaðt0Þ − ρbðt0ÞÞ
t0¼0
ð15Þ
for all possible pairs. The goal is to pick the first few
trajectories with minimum total distance to other trajecto
ries in the ensemble and average them to get an estimate of
the experimental most-likely paths. For this particular set of
data, we choose about 102 highly likely trajectories to get a
smooth estimate of the most-likely paths. However, for the
case in which there exist multiple (e.g., three) most-likely
paths, we first divide the ensemble into subensembles
according to their trace distance and then apply the
minimum total distance procedure to the trajectories in
each subensemble separately. In Figs. 3(a)–3(c), we show
the concurrence of the experimental most-likely paths as
data points.
Ideally, the theoretical most-likely paths predicted from
the log-likelihood density, Eq. (14), for each set of
measurement strengths using the initial state fx0
1;…;x0
5g¼
f1=4;…;1=4g would be good enough to compare with the
experimental data. However, in the experiment, after the
initial state has been prepared, the cavities take some time
(c)
(d)
(e)
(f)
FIG. 3. The most-likely paths from the theoretical prediction and the experimental data. The first, second, and third columns are from
three different data sets, measuring the same qubits and cavities with three different measurement-readout powers (indicated by the
characteristic measurement time): τm ¼ 2.10 μs, 0.60 μs, and 0.36 μs, respectively. Panels (a)–(c) show the concurrence of the multiple
most-likely paths: the path with high concurrence (solid purple line), and the two paths with low concurrence projecting onto j00i
(dashed orange line) and j11i (dotted green line) subspaces. The vertical lines (labeled as A1;2, B, C1;2, D) represent the times at which
the concurrence is maximum for each of these paths. The insets show the log-likelihood density as functions of optimal measurement
readouts, and the grey-scale histograms in the background show experimental concurrence histograms similar to the one in Fig. 2(c).
Panels (d)–(f) present the evolution of the density matrix elements of the high-concurrence most-likely paths: The solid curves indicate
theoretical solutions, whereas the data points indicate experimental most-likely paths postselected with the most entangled state at the
final time T ¼ 1.6 μs. Examples of the postselected trajectories are shown as fluctuating curves.
041052-8
QUANTUM TRAJECTORIES AND THEIR STATISTICS FOR …
PHYS. REV. X 6, 041052 (2016)
to reach their steady-state condition, making the parameters
δv1; …;δv4 unstable during the first ∼0.13 μs time.
Therefore, we need to let the initial qubit state evolve
and then find new “initial” states at time t ¼ 0.13 μs for the
theoretical most-likely path calculation. We use the exper
imental most-likely states at t ¼ 0.13 μs (one for each
branch) as the initial states in calculating the log-likelihood
density functions (the insets), which then leads to an
excellent prediction of the most-likely paths and their
concurrence for the rest of the evolution.
We also note that the two unequal low-concurrence
branches in Figs. 3(b) and 3(c) happen because the
population of the states drifts more toward the ground
state j00i during the transient time, as a result of the
qubit relaxation during the measurement. Moreover, in
Figs. 3(d)–3(f), we present the evolution of matrix elements
of the high-concurrence most-likely paths, showing a good
agreement between the theoretical most-likely paths and
experimental most-likely paths postselected with the most
entangled state at the final time T ¼ 1.6 μs.
B. Most-likely paths for perfectly
symmetric half-parity measurement
We are also interested in finding analytic solutions for
the most-likely paths for the symmetric case: δv2¼δv3¼0
and −δv1 ¼ δv4 ¼ δv. The differential equations (13) for
the qubit state simplify to
∂txp ¼ −bxp − axm þ axpxm þ bx2 p;
ð16aÞ
∂txm ¼−bxm −axp þbxmxp þax2m; ð16bÞ
∂tx2;3 ¼þx2;3ðaxm þ bxpÞ;
∂tx5 ¼−γx5 þx5ðaxm þ bxpÞ;
ð16cÞ
ð16dÞ
where we have defined new variables xp ≡x1 þx4 and
xm ≡x1 −x4, and constant parameters a ¼ vtδv=s and
b ¼δv2=4s. The first two equations can be solved inde
pendently from the rest. For the case vt ¼ δv2;3 ¼ 0, which
corresponds to the most-likely odd-parity result, we obtain
an analytic solution for the high-concurrence branch of the
most-likely path,
x1;4ðtÞ ∝ x0
1;4 expð−δv2t=4sÞ;
x2;3ðtÞ ∝ x0
2;3;
x5ðtÞ ∝ x0
5 expð−γtÞ;
ð17aÞ
ð17bÞ
ð17cÞ
where the proportionality factor is the inverse of a normal
ized factor N ¼ð1 −x0
1 −x0
4Þþðx0
1 þ x0
4Þexpð−δv2t=4sÞ.
The concurrence of this path exactly coincides with the
upper concurrence bound derived in Eq. (11), which is not
surprising because the distribution of concurrence shows
sharp peaks along the concurrence bound. We note that the
solutions for the low-concurrence branch (for vt ¼ δv and
vt ¼ −δv) can be found numerically.
In the above analysis, for the half-parity case, a simple
analytic solution for the most-likely path for arbitrary
values of vt was not forthcoming. However, if we further
simplify the problem by considering a parity meter [6], then
we can solve the equations of motion, Eqs. (13) and their
conjugate equations, exactly. A parity meter has the same
detector outputs for the even- and odd-parity subspaces, but
the detector can distinguish between the subspaces. More
detail of the calculation is presented in Appendix C.
C. Distribution of time to maximum concurrence
In the process of the entanglement generation, there are
interesting quantities to investigate, such as the maximum
concurrence each individual trajectory can reach and the
time it takes to reach the highest value. We previously
showed that qubit trajectories branch out to high- and low
concurrence subspaces. Therefore, one would expect that
there are two most-likely times for the qubit trajectories to
reach their maximum concurrences (or their most entangled
states).
In Fig. 4, we show the normalized histograms of time for
transmon qubit trajectories to reach their maximum con
currence. The histograms for the τm ¼ 0.36 μs and 0.60 μs
measurement cases explicitly show double peaks, which
agree with the branching of concurrence and the most
likely qubit paths in Figs. 3(b) and 3(c). The times at which
these peaks are located can be theoretically predicted from
FIG. 4. Histograms of the time to maximum concurrence for
individual trajectories for three measurement strengths indicated
by the values of τm. For the two cases with strong readout powers
(shown in red and green histograms), there exists two peaks
corresponding to two most-likely times to reach their most
entangled states. The theoretical predictions of these times are
shown as vertical dashed lines labeled as A1;2, B, C1;2, D [same as
in Figs. 3(a)–3(c)].
041052-9
AREEYA CHANTASRI et al.
PHYS. REV. X 6, 041052 (2016)
the time to maximum concurrence of the solutions of the
most-likely paths. As shown by the vertical dashed lines in
Figs. 3(b), 3(c), and 4, A1;2 and B are the two most-likely
times to reach maximum concurrence (for low- and high
concurrence branches, respectively) for τm ¼ 0.60 μs, and
C1;2 and D are the same but for the case with τm ¼ 0.36 μs.
The agreement between the theoretical prediction of the
peaks and the peaks of the histograms are as good as the
agreement of the theory-experiment most-likely paths in
Figs. 3(b) and 3(c). We note that for the weak measurement
regime, τm ¼ 2.10 μs, the bifurcation has not occurred yet
during the measurement time T ¼ 1.6 μs. One would
expect to see a branching effect when the total measure
ment time is long enough.
V. CONCLUSION
We have investigated the process of entanglement gen
eration between two spatially separated superconducting
transmon qubits and their statistical properties. The entan
glement of the two qubits is created as a result of the half
parity dispersive measurement via the microwave pulses
sequentially interacting with both qubits. The strength of
the joint measurement is arbitrary, and we have studied
three different values of the measurement strength. We
examined the concurrence of individual trajectories and
theoretically calculated its distribution from the quantum
Bayesian approach, gradually projecting the two-qubit
states to entangled states with high concurrence and to
separable states with zero concurrence.
The most-likely path analysis was also carried out,
predicting the most probable paths for the qubit trajectories.
We found that in the two-qubit-state space, there are three
likely paths conforming to the three branches projecting to
the j00i subspace, the j11i subspace, and the odd (j01i,
j10i) subspaces; the first two correspond to the lower
branches of the concurrence bifurcation, and the last
corresponds to the high-concurrence branch. These theo
retical most-likely paths show good agreement with the
experimental most-likely ones extracted from the transmon
trajectory data (for three independent data sets) based on
the trace distance between trajectories in two-qubit-state
space. Moreover, we have presented the distributions of the
time to the maximum concurrence for individual trajecto
ries. The most-likely path analysis was shown to be useful
in predicting the peaks of these time distributions.
We conclude that the accurate tracking of quantum
trajectories of a jointly measurement qubit system is
possible and that the physics of the entanglement creation
statistics is well described by a quantum trajectory theo
retical approach. The theoretical most-likely paths to
entanglement and concurrence distribution match the
experiment excellently. This work shows the way to use
this process as a control mechanism to entangle remote
systems for quantum-information-processing purposes.
In future work, similar questions can be posed about the
full-parity measurement, and we have made some predic
tions about that case in this work.
ACKNOWLEDGMENTS
This work was supported by US Army Research Office
Grants No. W911NF-15-1-0496 and No. W911NF-13-1
0402, by National Science Foundation Grant No. DMR
1506081, by John Templeton Foundation Grant ID 58558,
and by the Development and Promotion of Science and
Technology Talents Project Thailand. M. E. K. S. acknowl
edges support from the Fannie and John Hertz Foundation.
APPENDIX A: OPTIMIZED PATHS (MOST
LIKELY PATHS) WITH PRESELECTED OR
POSTSELECTED STATES
We follow the outline in Refs. [36,37] for the stochastic
path-integral formalism and the action principle for con
tinuous quantum measurement. A joint probability density
function of quantum states and measurement readouts,
from time t0 ¼ 0 to t0 ¼ t, is given by a path integral
Z
Pðfxtg;fvtgjx0Þ¼N
Z t
S ¼−
DpðtÞexpS;
5
ðvt0 − δviÞ2xi þ 
X
ðA1Þ
pjð∂t0xj − FjÞ ;
0
dt0 1
s
X4
i¼1
j¼1
ðA2Þ
where fxtg¼fxj;t0g denotes a set of quantum-state matrix
elements at all times (with j ¼ 1;2;…;5, and t0 runs from
time t0 ¼ 0 to t0 ¼ t), and DpðtÞ denotes the path-integral
measure for the conjugate variables (or Lagrange multi
pliers as mentioned in the main text). The action of the
path integral S [37] is given in terms of the two-qubit
density matrix variables xj and their conjugates pj for
j ¼1;2;…;5, which are implicitly functions of time t0.
The first sum in the time integral of S is the logarithm of the
joint probability density function of the measurement
readout PðfvtgÞ, Eq. (12), truncated to first order in δt
(taking a time continuum limit), and the functional Fj is the
right-hand side of Eq. (13).
The joint probability density function in a path-integral
representation, Eq. (A2), is written with a measure
DxðtÞDvðtÞ ≡ limδt→0 
Qt
t0¼0 dx1;t0dx2;t0 
dx5;t0dvt0 , con
sidering the density matrix elements and the measurement
readout as random variables. The probability density
function multiplied by the measure gives a probability that
is vanishingly small but invariant under changes of mea
sure. However, as in usual probability theory, one can ask
about “peaks” or the most-likely values of an associated
probability density function. The most-likely paths for the
quantum trajectories starting from an initial state and
041052-10
QUANTUM TRAJECTORIES AND THEIR STATISTICS FOR …
PHYS. REV. X 6, 041052 (2016)
ending at a final state after some time t can be found by
optimizing the action of the stochastic path integral (A2).
By extremizing the action Eq. (A2) over all variables xi,
pi, vt, we get a set of ten ordinary differential equations
(ODEs) for the optimized path, and one equation for
optimal measurement readout. The set of ODEs includes
five differential equations of the two-qubit variables xi,as
shown in Eq. (13), and five equations for the conjugate
variables pi,
X4
∂tpi ¼
where
j¼1
xjAij þ x5p5Bi þ Ci
∂tp5 ¼þγ5p5 þp5
for i ¼ 1;2;3;4;
ðA3aÞ
X4
j¼1
xjBj;
Aij ¼ −ðpi −pjÞð2vt −δvi −δvjÞðδvi − δvjÞ;
ðA3bÞ
Bi ¼ 1
2s fvtð4δvi − 2δv2 − 2δv3Þ − ð2δv2
i − δv2
2 − δv2
3Þg;
Ci ¼ 1
2s ðvt − δviÞ2:
The optimal readout is given as a function of the two-qubit
variables and the conjugate variables,
X4
vt ¼
i¼1
X4
fpixixjðδvi − δvjÞþxiδvig
j¼1
þp5x5
2
X4
ðδv2 þ δv3 −2xiδviÞ;
i¼1
ðA4Þ
connecting the ODEs for the qubit variables and the
conjugate variables. We note that by taking a time deriva
tive of the function in Eq. (A4) and substituting both ∂txi
and ∂tpj with the ODEs above, we find that ∂tvt ¼ 0,
therefore implying that an optimal readout is a constant
in time.
From the joint probability density function (A1), we can
consider integrating out the measurement-readout variables
to get a probability density function just in the quantum
state
variables,
i.e.,
Pðfxtgjx0Þ¼R DvðtÞPðfxtg;
fvtgjx0Þ. Since the action (A2) is bilinear in vt, its
Gaussian-functional integral gives exactly the same result
(up to a constant normalization factor) as extremizing the
action over the readout and substituting the optimal
solution (A4) to the action. By extremizing the rest of
the action over the quantum-state variables and their
conjugates, we get the same set of ten differential equa
tions [Eqs. (13) and (A3)] with the substitution of the
optimal readout (A4). The solutions to these equations can
now be interpreted as an optimal path in the quantum-state
space only. This similar definition of the optimal path
is also used in classical stochasticprocesses, for example,by
the variation of the Martin-Siggia-Rose action formalism
[56,57].
APPENDIX B: TRANSFORMATION OF THE
MOST-LIKELY PATH UNDER CHANGE
OF MEASURE
We further investigate the transformations of the optimal
paths under change of measure. In probability theory, given
a probability density function of a continuous random
variable V, one can consider a change of variable
V →ζ¼gðVÞ, where ζ is a new random variable. The
total probability contained in the differential region should
be invariant, i.e., pVðVÞdV ¼ pζðζÞdζ, so the new prob
ability density function can be reformulated as
pζðζÞ¼pVðg−1ðζÞÞj½d=ðdζÞg−1ðζÞj, assuming that g is
monotonic. If there exists an optimal value Vopt, obtained
by solving ½d=ðdVÞpVðVÞjVopt 
¼ 0, and there similarly
exists an optimal value in the ζ variable, one can show
that ζopt does not need to be the same as gðVoptÞ. Thus, a
question regarding an optimal (most-likely) value is de
pendent on the random variables one is interested in; that is,
it is measure dependent. We also note that for a special case
when gðVÞ is a linear function, the optimal values in the
two variables coincide, ζopt ¼ glinearðVoptÞ.
We stress that, even though the joint optimization of the
quantum states and the measurement readouts (A1) can
give a different solution under a change of the readout
variables, we can avoid this change of measure by
integrating out all the readout variables and only consid
ering the optimal path in the quantum-state space, as
discussed at the end of the previous appendix. For the
rescaled shifted homodyne signal as a readout variable, the
joint optimization happens to coincide with the quantum
state optimization after integrating out the readout varia
bles. This way we have thus proven that our quantum-state
optimal path is independent of the readout measure, while
the optimal readout itself vt is a measure-dependent
quantity in general.
APPENDIX C: ANALYTIC SOLUTION IN THE
CASE OF A PARITY METER
For the full-parity measurement case, we assume
δv1 ¼ δv4 ¼ dv, while δv2 ¼ δv3 ¼ 0. With this special
case, we find the equations of motion
∂tx1 ¼þλx1xo;
∂tx2 ¼ −λx2xe;
∂tx3 ¼ −λx3xe;
∂tx4 ¼þλx4xo;
ðC1aÞ
ðC1bÞ
ðC1cÞ
ðC1dÞ
041052-11
AREEYA CHANTASRI et al.
ðC1eÞ
PHYS. REV. X 6, 041052 (2016)
∂tx5 ¼−γx5 −λx5xe;
wherewe define λ ¼ 2vtδv=s − δv2=s,andxe ¼ x1 þx4 ¼
ρ00;00 þ ρ11;11 is the probability of being in the even-parity
subspace, while xo ¼ x2 þ x3 ¼ ρ01;01 þ ρ10;10 is the prob
ability of being in the odd-parity subspace.
Taking the sum of ∂tx1 and ∂tx4, we can derive an
equation for xo alone since xe þ xo ¼ 1,
_
xo ¼ −_xe ¼ −λð1−xoÞxo:
Integrating this equation gives the solution
xoðtÞ¼
x0 oe−λt
1 −x0 oð1 − e−λtÞ ;
ðC2Þ
ðC3Þ
where x0 o is the initial condition for x2 þ x3. Similarly, we
find for the even probability,
xeðtÞ¼
x0 e
1 −x0 oð1 − e−λtÞ ;
ðC4Þ
where x0 e is the initial condition for x1 þ x4.
Notice that the value of λ may be found completely from
these results. The parity probability of the initial prese
lected and final postselected states will fix the value of λ.If
the integrated signal gives a positive answer larger than
dv=2, λ will be positive, tending to collapse the state into
the even-parity subspace. Conversely, if the integrated
signal is less than dv=2, then λ will be negative, tending
to collapse the system into the odd-parity subspace.
From these solutions, we may find the other density
matrix solutions. For example, Eq. (C1a) may be rewritten
as ∂t ln x1 ¼ λxo, which can be integrated to get
x1ðtÞ¼x0
1 expfλR t
0 dt0xoðt0Þg. We simply apply this
method to the rest of Eqs. (C1) and obtain the solutions,
the most-likely path of the two-qubit problem,
x1ðtÞ¼
x0
1
1 −ðx0
2 þ x0
3Þð1 − e−λtÞ ;
x2ðtÞ¼
x0
2e−λt
1 −ðx0
2 þ x0
3Þð1 − e−λtÞ ;
x3ðtÞ¼
x0
3e−λt
1 −ðx0
2 þ x0
3Þð1 − e−λtÞ ;
x4ðtÞ¼
x0
4
1 −ðx0
2 þ x0
3Þð1 − e−λtÞ ;
x5ðtÞ¼
x0
5e−ðγþλÞt
1 −ðx0
2 þ x0
3Þð1 − e−λtÞ ;
ðC5aÞ
ðC5bÞ
ðC5cÞ
ðC5dÞ
ðC5eÞ
where the value of λ can be fixed once we have specified the
initial and final values of the density matrix, x0
1;x0
2;…;
x0
5;x1;f;x2;f; …;x5;f.
Finally, we may find the concurrence of the most-likely
path by calculating C ¼ 2 maxf0;x5 − ffiffiffiffiffiffiffiffiffi
x1x4
p g.Wefindthe
result
p
ffiffiffiffiffiffiffiffiffi
x0
5je−ðγþλÞtj −
x0
1x0
4
CðtÞ¼2max 0;
j1 −ðx0
2 þ x0
3Þð1 − e−λtÞj :
ðC6Þ
In order to cross the entanglement border [6] from an
unentangled state, λ must take on a negative value to
enhance the first term over the second, taking the system
into the odd-parity subspace.
The entanglement border will be crossed when the
concurrence is zero or when the condition
x0
5
γ þλ ¼ð1=tÞln
ffiffiffiffiffiffiffiffiffiffiffiffi
p ðC7Þ
jx0
1x0
4j
is satisfied.
[1] C. K. Hong, Z.Y. Ou, and L. Mandel, Measurement of
Subpicosecond Time Intervals between Two Photons by
Interference, Phys. Rev. Lett. 59, 2044 (1987).
[2] A.N. Korotkov, Continuous Measurement of Entangled
Qubits, Phys. Rev. A 65, 052304 (2002).
[3] R. Ruskovand A.N. Korotkov, Entanglement of Solid-State
Qubits by Measurement, Phys. Rev. B 67, 241305 (2003).
[4] W. Mao, D.V. Averin, R. Ruskov, and A.N. Korotkov,
Mesoscopic Quadratic Quantum Measurements, Phys. Rev.
Lett. 93, 056803 (2004).
[5] B. Trauzettel, A. N. Jordan, C.W.J. Beenakker, and M.
Büttiker, Parity Meter for Charge Qubits: An Efficient
Quantum Entangler, Phys. Rev. B 73, 235331 (2006).
[6] N.S. Williams and A.N. Jordan, Entanglement Genesis
under Continuous Parity Measurement, Phys. Rev. A 78,
062322 (2008).
[7] S. G. Hofer, D.V. Vasilyev, M. Aspelmeyer, and K.
Hammerer, Time-Continuous Bell Measurements, Phys.
Rev. Lett. 111, 170404 (2013).
[8] C. W. Chou, H. de Riedmatten, D. Felinto, S.V. Polyakov,
S. J. van Enk, and H.J. Kimble, Measurement-Induced
Entanglement for Excitation Stored in Remote Atomic
Ensembles, Nature (London) 438, 828 (2005).
[9] D.L. Moehring, P Maunz, S Olmschenk, K.C. Younge,
D. N. Matsukevich, L.-M. Duan, and C. Monroe, Entangle
ment of Single-Atom Quantum Bits at a Distance, Nature
(London) 449, 68 (2007).
[10] H. Bernien, B. Hensen, W. Pfaff, G. Koolstra, M. S. Blok, L.
Robledo, T. H. Taminiau, M. Markham, D.J. Twitchen, L.
Childress, and R. Hanson, Heralded Entanglement between
Solid-State Qubits Separated by Three Metres, Nature
(London) 497, 86 (2013).
[11] B. Hensen, H. Bernien, A.E. Dréau, A. Reiserer, N. Kalb,
M.S. Blok, J. Ruitenberg, R.F.L. Vermeulen, R.N.
041052-12
QUANTUM TRAJECTORIES AND THEIR STATISTICS FOR …
PHYS. REV. X 6, 041052 (2016)
Schouten, C. Abellán et al., Loophole-Free Bell Inequality
Violation Using Electron Spins Separatedby 1.3 Kilometres,
Nature (London) 526, 682 (2015).
[12] N. Roch, M.E. Schwartz, F. Motzoi, C. Macklin, R. Vijay,
A. W. Eddins, A.N. Korotkov, K.B. Whaley, M. Sarovar,
and I. Siddiqi, Observation of Measurement-Induced
Entanglement and Quantum Trajectories of Remote
Superconducting Qubits, Phys. Rev. Lett. 112, 170501
(2014).
[13] M.H. Devoret and R.J. Schoelkopf, Superconducting
Circuits for Quantum Information: An Outlook, Science
339, 1169 (2013).
[14] K.W. Murch, R. Vijay, and I. Siddiqi, Weak Measurement
and Feedback in Superconducting Quantum Circuits, in
Superconducting Devices in Quantum Optics, edited by
Robert H. Hadfield and Göran Johansson (Springer
International Publishing, Switzerland, 2016), pp. 163–185.
[15] J. Ghosh, A. Galiautdinov, Z. Zhou, A. N. Korotkov, J. M.
Martinis, and M.R. Geller, High-Fidelity Controlled-σZ
Gate for Resonator-Based Superconducting Quantum
Computers, Phys. Rev. A 87, 022309 (2013).
[16] A. Fedorov, L. Steffen, M. Baur, M.P. Da Silva, and A.
Wallraff, Implementation of a Toffoli Gate with Super
conducting Circuits, Nature (London) 481, 170 (2011).
[17] M. Ansmann, H. Wang, R.C. Bialczak, M. Hofheinz,
E. Lucero, M. Neeley, A. D O’Connell, D. Sank, M.
Weides, J. Wenner et al., Violation of Bell’s Inequality in
Josephson Phase Qubits, Nature (London) 461, 504 (2009).
[18] R. C. Bialczak, M. Ansmann, M. Hofheinz, E. Lucero,
M. Neeley, A.D. O’Connell, D. Sank, H. Wang, J. Wenner,
M. Steffen et al., Quantum Process Tomography of a
Universal Entangling Gate Implemented with Josephson
Phase Qubits, Nat. Phys. 6, 409 (2010).
[19] B. Vlastakis, G. Kirchmair, Z. Leghtas, S.E. Nigg,
L. Frunzio, S. M. Girvin, M. Mirrahimi, M.H. Devoret,
and R.J. Schoelkopf, Deterministically Encoding Quantum
Information Using 100-Photon Schrödinger Cat States,
Science 342, 607 (2013).
[20] M.A. Castellanos-Beltran, K. D. Irwin, G. C. Hilton, L. R.
Vale, and K.W. Lehnert, Amplification and Squeezing of
Quantum Noise with a Tunable Josephson Metamaterial,
Nat. Phys. 4, 929 (2008).
[21] M. Hatridge, R. Vijay, D.H. Slichter, John Clarke, and
I. Siddiqi, Dispersive Magnetometry with a Quantum
Limited SQUID Parametric Amplifier, Phys. Rev. B 83,
134501 (2011).
[22] N. Katz, M. Ansmann, R.C. Bialczak, E. Lucero, R.
McDermott, M. Neeley, M. Steffen, E.M. Weig, A.N.
Cleland, J. M. Martinis, and A. N. Korotkov, Coherent State
Evolution in a Superconducting Qubit from Partial
Collapse Measurement, Science 312, 1498 (2006).
[23] A.N. Korotkov and A.N. Jordan, Undoing a Weak Quan
tum Measurement of a Solid-State Qubit, Phys. Rev. Lett.
97, 166805 (2006).
[24] N. Katz, M. Neeley, M. Ansmann, R.C. Bialczak,
M. Hofheinz, E. Lucero, A. O’Connell, H. Wang, A.N.
Cleland, J. M. Martinis, and A.N. Korotkov, Reversal
of the Weak Measurement of a Quantum State in a Super
conducting Phase Qubit, Phys. Rev. Lett. 101, 200401
(2008).
[25] J. P. Groen, D. Ristè, L. Tornberg, J. Cramer, P. C. de Groot,
T. Picot, G. Johansson, and L. DiCarlo, Partial
Measurement Backaction and Nonclassical Weak Values
in a Superconducting Circuit, Phys. Rev. Lett. 111, 090506
(2013).
[26] P. Campagne-Ibarcq, L. Bretheau, E. Flurin, A. Auffèves,
F. Mallet, and B. Huard, Observing Interferences between
Past and Future Quantum States in Resonance Fluores
cence, Phys. Rev. Lett. 112, 180402 (2014).
[27] N.S. Williams and A.N. Jordan, Weak Values and the
Leggett-Garg Inequality in Solid-State Qubits, Phys. Rev.
Lett. 100, 026804 (2008).
[28] H.M. Wiseman and G.J. Milburn, Quantum Measurement
and Control (Cambridge University Press, Cambridge,
England, 2010).
[29] R. Vijay, C. Macklin, D.H. Slichter, S.J. Weber, K.W.
Murch, R. Naik, A.N. Korotkov, and I. Siddiqi, Stabilizing
Rabi Oscillations in a Superconducting Qubit Using Quan
tum Feedback, Nature (London) 490, 77 (2012).
[30] G. de Lange, D. Ristè, M.J. Tiggelman, C. Eichler,
L. Tornberg, G. Johansson, A. Wallraff, R.N. Schouten,
and L. DiCarlo, Reversing Quantum Trajectories with
Analog Feedback, Phys. Rev. Lett. 112, 080501 (2014).
[31] K.W. Murch, S.J. Weber, C. Macklin, and I. Siddiqi,
Observing Single Quantum Trajectories of a Superconduct
ing Quantum Bit, Nature (London) 502, 211 (2013).
[32] A.N. Jordan, Quantum Physics: Watching the Wavefunc
tion Collapse, Nature (London) 502, 177 (2013).
[33] P. Campagne-Ibarcq, P. Six, L. Bretheau, A. Sarlette, M.
Mirrahimi, P. Rouchon, and B. Huard, Observing Quantum
State Diffusion by Heterodyne Detection of Fluorescence,
Phys. Rev. X 6, 011002 (2016).
[34] M.Naghiloo, N. Foroozani, D. Tan, A. Jadbabaie, and K. W.
Murch, Mapping Quantum State Dynamics in Spontaneous
Emission, Nat. Commun. 7, 11527 (2016).
[35] S. J. Weber, A. Chantasri, J. Dressel, A. N. Jordan, K. W.
Murch, and I. Siddiqi, Mapping the Optimal Route between
Two Quantum States, Nature (London) 511, 570 (2014).
[36] A. Chantasri, J. Dressel, and A. N. Jordan, Action Principle
for Continuous Quantum Measurement, Phys. Rev. A 88,
042110 (2013).
[37] A. Chantasri and A.N. Jordan, Stochastic Path-Integral
Formalism for Continuous Quantum Measurement, Phys.
Rev. A 92, 032125 (2015).
[38] A.N. Jordan, A. Chantasri, P. Rouchon, and B. Huard,
Anatomy of Fluorescence: Quantum Trajectory Statistics
from Continuously Measuring Spontaneous Emission,
Quantum Stud. Math. Found. 3, 237 (2016).
[39] G. Haack, H. Förster, and M. Büttiker, Parity Detection and
Entanglement with a Mach-Zehnder Interferometer, Phys.
Rev. B 82, 155303 (2010).
[40] F. Helmer and F. Marquardt, Measurement-Based Synthesis
of Multiqubit Entangled States in Superconducting Cavity
QED, Phys. Rev. A 79, 052328 (2009).
[41] K. Lalumière, J. M. Gambetta, and A. Blais, Tunable Joint
Measurements in the Dispersive Regime of Cavity QED,
Phys. Rev. A 81, 040301 (2010).
[42] J. Wang, H.M. Wiseman, and G.J. Milburn, Dynamical
Creation of Entanglement by Homodyne-Mediated Feed
back, Phys. Rev. A 71, 042309 (2005).
041052-13
AREEYA CHANTASRI et al.
PHYS. REV. X 6, 041052 (2016)
[43] C. Hill and J. Ralph, Weak Measurement and Control of
Entanglement Generation, Phys. Rev. A 77, 014305 (2008).
[44] C. Meyer zu Rheda, G. Haack, and A. Romito, On-Demand
Maximally Entangled States with a Parity Meter and
Continuous Feedback, Phys. Rev. B 90, 155438 (2014).
[45] D. Riste, M. Dukalski, C.A. Watson, G. de Lange, M.J.
Tiggelman, Ya. M. Blanter, K. W. Lehnert, R. N. Schouten,
and L. DiCarlo, Deterministic Entanglement of Supercon
ducting Qubits by Parity Measurement and Feedback,
Nature (London) 502, 350 (2013).
[46] F. Motzoi, K. B. Whaley, and M. Sarovar, Continuous Joint
Measurement and Entanglement of Qubits in Remote
Cavities, Phys. Rev. A 92, 032308 (2015).
[47] L. Martin, F. Motzoi, H. Li, M. Sarovar, and K. B. Whaley,
Deterministic Generation of Remote Entanglement with
Active Quantum Feedback, Phys. Rev. A 92,062321(2015).
[48] J. Govenius, Y. Matsuzaki, I. G. Savenko, and M. Möttönen,
Parity Measurement of Remote Qubits Using Dispersive
Coupling and Photodetection, Phys. Rev. A 92, 042305
(2015).
[49] M. Silveri, E. Zalys-Geller, M. Hatridge, Z. Leghtas, M. H.
Devoret, and S. M. Girvin, Theory of Remote Entanglement
via Quantum-Limited Phase-Preserving Amplification,
Phys. Rev. A 93, 062310 (2016).
[50] A. Narla, S. Shankar, M. Hatridge, Z. Leghtas, K. Sliwa, E.
Zalys-Geller, S. Mundhada, W. Pfaff, L. Frunzio, R.
Schoelkopf, and M. Devoret, Robust Concurrent Remote
Entanglement between Two Superconducting Qubits, Phys.
Rev. X 6, 031036 (2016).
[51] A.N. Jordan and A.N. Korotkov, Qubit Feedback and
Control with Kicked Quantum Nondemolition Measure
ments: A Quantum Bayesian Analysis, Phys. Rev. B 74,
085307 (2006).
[52] Theoretically, if there is no single-qubit unitary rotation and
the initial matrix elements are real values, all elements
would stay real during the measurement process. However,
in the experiment, the two cavities are not exactly at the
same frequency and the qubits are not equally coupled to
their respective cavities, so the qubits experience different
ac-Stark shifts. The off-diagonal element acquires a deter
ministic (i.e., predictable) nonzero phase that increases
linearly in time and, critically, does not affect the degree
of entanglement in the system. We therefore study the
magnitude of this element and neglect the phase.
[53] J. M. Chow, L. DiCarlo, J.M. Gambetta, A. Nunnenkamp,
L. S. Bishop, L. Frunzio, M. H. Devoret, S. M. Girvin, and
R. J. Schoelkopf, Detecting Highly Entangled States with a
Joint Qubit Readout, Phys. Rev. A 81, 062325 (2010).
[54] W.K. Wootters, Entanglement of Formation of an Arbitrary
State of Two Qubits, Phys. Rev. Lett. 80, 2245 (1998).
[55] L. Jakbczyk and A. Jamrz, Generation of Werner States and
Preservation of Entanglement in a Noisy Environment,
Phys. Lett. A 347, 180 (2005).
[56] P. C. Martin, E.D. Siggia, and H.A. Rose, Statistical
Dynamics of Classical Systems, Phys. Rev. A 8, 423
(1973).
[57] A. Kamenev, Field Theory of Non-Equilibrium Systems
(Cambridge University Press, Cambridge, England, 2011).
041052-14