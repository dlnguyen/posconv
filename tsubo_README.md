TSUBOGURUMA by Hiroaki Nissho

Kihonteki tsukaikata: tsubo.pl --command <POSCAR

Commands:

-h -help --help : Help wo hyouji
--version : Version wo hyouji

--clat : a,b,c,alpha,beta,gamma kara lattice vector wo tsukuru (POSCAR iranai)

--data : kousi teisuu nado wo hyouji
--dataniggli : niggli reduced cell no kousi teisuu nado wo hyouji
--natoms --numatoms : Gensi no kazu wo hyouji
--nspecies --numspecies : Genso no kazu wo hyouji
--dist D : Kyori D ika no gensi wo hyouji
--dist_large D : Kyori D ika no gensi wo hyouji (kensaku hanni wo hirogeru)
--dist_min : Saisyou genshikan kyori wo hyouji
--nameatom N : gensi N no gensomei (6 gyome) to genso bango (7 gyome) wo kaesu
--sgnumber : Kuukan gun bangou wo kaesu
--sgsymbol : Kuukan gun symbol wo kaesu
--pgsymbol : Ten gun symbol wo kaesu
--crystalsystem : Kesshou kei wo kaesu (Triclinic nado)
--bravais : Bravais lattice wo kaesu (aP nado)
--sclatticetype : Kousi no shurui wo kaesu (eg CUB, ORCF2)
--normal_vector H K L length : HKL hyoumen ni suichoku de nagasa length no vector wo hyouji
--isometry : Subete no isometry wo hyouji
--surface_isometry H K L [asis] : HKL hyoumen no slab no taisyousei wo
hyouji
--unique_nonpolar [h k l] [cap] : nonpolar surface wo chiisai jun ni kaesu
--termination_polarity H K L [asis] : HKL hyoumen no slab no osusume wo hyouji
--termination_polarity_full H K L [asis] : HKL hyoumen no slab no polarity wo hyouji
--termination_polarity_list file : file no hyoumen no slab no polarity wo hyouji
--2ddiffraction H K L : H K L houkou no 2D diffraction pattern wo kaesu

--scale A : POSCAR no kousi teisuu wo A bai suru
--scale A B C: POSCAR no kousi teisuu wo sorezore A,B,C bai suru
--scalexyz A B C: POSCAR no x,y,z zahyo wo A,B,C bai suru
--rotate_axis abc: POSCAR no kitei vector wo mawasu
--hklcell_supercell --hkl_supercell H K L [asis] : HKL houkou no supercell wo tsukuru
--hklcell_primitive --hkl_primitive H K L [asis] : HKL houkou no primitive cell wo tsukuru
--slab_poscar slab_thickness vacuum_thickness H K L [asis] : HKL hyoumen no slab wo kaesu
--slab_poscar_directory slab_thickness vacuum_thickness H K L [asis] : directory wo tsukutte HKL hyoumen no slab wo kaesu";
--slab_poscar_list slab_thickness vacuum_thickness file : directory wo tsukutte file no hyoumen no slab wo kaesu";

--species --names A B C ... : Genso no namae wo sitei (kaku gensi, 9+ gyou me)
--species6 --names6 A B C ... : Genso no namae wo sitei (6 gyo me)
--noelement ... : Genso no namae wo 9 gyou me ikou hyouji sinai

--incell : Subete no zahyou wo 0 to 1 no aida ni suru
--frac -f -d --fract --fractional --direct : Direct kara Cartesian ni suru
--cart -c : Cartesian kara Direct ni suru
--shift A B C : site wo zenbu (A,B,C) dake zurasu
--swap_atom A B : A-banme gensi to B-banme gensi no ichi dake wo koukansuru (genso ha koukan sinai)
--swap_species A B : A-banme genso to B-banme genso wo koukan suru
--similar POSCAR1 : POSCAR1 ni chikai zahyo no POSCAR wo kaesu
--nebimages POSCAR1 N : NEB you ni 00 kara N+1 made POSCAR image wo kaesu

--niggli:  POSCAR no niggli reduced cell wo tsukuru (POSCAR ha primitive to site atukau = primitive wo sagasanai!)
--reciniggli : POSCAR no gyaku kousi ga niggli reduced cell ni naru youni suru
--maxortho : POSCAR no c jiku wo a, b jiku ni taisi maximally orthogonal ni suru

--unique : POSCAR no tyouhuku suru saito wo hitotu ni suru
--makeslab minz maxz shiftz tolerance : z zahyou ga minz - maxz no sla wo tsukuru,	hituyou nara shiftz dake zurasu
--rm_atom A B C..D .. : gensi A B C..D .. wo kesu, gensi ha ikutu sitei sitemo ii, gensi ha 1 kara kazoeru
--rm_species A B C..D .. : gensi A B C..D .. wo kesu, gensi ha ikutu sitei sitemo ii, genso ha 1 kara kazoeru

--supercell A B C : POSCAR no supercell wo tukuru
--supercell A1 A2 A3 B1 B2 B3 C1 C2 C3 : POSCAR no supercell wo tukuru
--supercell [file] : POSCAR no supercell wo tukuru (matrix wo file ni ireru)
--addatom x y z (namae) : POSCAR no saigo ni ichi (x,y,z) no gensi wo\n tasu, genso no namae ha (namae), namae ha shouryaku kanou	
--addimages minx maxx miny maxy minz maxz : xyz muke ni gensi wo tasu

--cif : POSCAR wo P1 space group CIF ni suru, gensomei wa 6 gyome de uwagaki sinai!
--cif6 : POSCAR wo P1 space group CIF ni suru, gensomei wa 6 gyome de uwagaki!
--xyz : POSCAR wo xyz ni suru, gensomei wa 6 gyome de uwagaki sinai!
--xyz6 : POSCAR wo xyz ni suru, gensomei wa 6 gyome de uwagaki!

--cc --crystallographic_conventional --conventional --bposcar : Kessyougaku  *conventional* wo tsukuru
--cp --crystallographic_primtive : Kessyougaku  *primitive* wo tsukuru
--hinuma_reduced : Hinuma reduced triclinic cell wo tsukuru
--sc --standard_conventional : Standard *conventional* wo tsukuru
--sp --standard_primtive : Standard *primitive* wo tsukuru
--bzpoint [filename] : Brillouin zone no ten (kessyougaku ver) wo KPOINTS teki ni hyouji
--bzpoint_notrs [filename] : Brillouin zone no ten (no time reversal symmetry) wo KPOINTS teki ni hyouji
--scbzpoint [filename] : Brillouin zone no ten (SC ver) wo KPOINTS teki ni hyouji
--scpointkpf [filename] : Brillouin zone no ten (kessyougaku ver) wo kpf teki ni hyouji
--bzpointkpf [filename] : Brillouin zone no ten wo kpf teki ni hyouji
--bzpointkpf_notrs [filename] : Brillouin zone no ten (no time reversal symmetry) wo kpf teki ni hyouji
--scbzpointkpf [filename] : Brillouin zone no ten (SC ver) wo kpf teki ni hyouji
--kpath [interval] [filename] : suishyou kpath (kessyougaku ver) wo KPOINTS teki ni hyouji
--kpath_notrs [interval] [filename] : suishyou kpath (no time reversal symmetry) wo KPOINTS huu ni hyouji
--sckpath [interval] [filename] : suishyou kpath (SC ver) wo KPOINTS teki ni hyouji
--kpathkpf [filename] : suishyou kpath (kessyougaku ver) wo kpf teki ni hyouji
--kpathkpf_notrs [filename] : suishyou kpath (no time reversal symmetry) wo kpf teki ni hyouji
--sckpathkpf [filename] : suishyou kpath (SC ver) wo kpf teki ni hyouji
--kpathphonopy [filename] : suishyou kpath (kessyougaku ver) wo phonopy teki ni hyouji
--sckpathphonopy [filename] : suishyou kpath (SC ver) wo phonopy teki ni hyouji
--kpath_band [filename] : interval 0.025 kpath (kessyougaku ver) wo hyouji
--kpath_band_notrs [filename] : interval 0.025 kpath (no time reversal symmetry) wo hyouji
--sckpath_band [filename] : interval 0.025 kpath (SC ver) wo hyouji
--kpath_mass [filename] : yuukou situryou you 0.002 kpath (kessyougaku ver) wo hyouji
--kpath_mass_notrs [filename] : yuukou situryou you 0.002 kpath (no time reversal symmetry) wo hyouji
--sckpath_mass [filename] : yuukou situryou you 0.002 kpath (SC ver) wo hyouji
