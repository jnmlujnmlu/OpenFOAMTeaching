/*--------------------------------*- C++ -*----------------------------------*\
| =========                 |                                                 |
| \\      /  F ield         | OpenFOAM: The Open Source CFD Toolbox           |
|  \\    /   O peration     | Version:  2.3.0                                 |
|   \\  /    A nd           | Web:      www.OpenFOAM.org                      |
|    \\/     M anipulation  |                                                 |
\*---------------------------------------------------------------------------*/
FoamFile
{
    version     2.0;
    format      ascii;
    class       dictionary;
    object      blockMeshDict;
}
// * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * * //

convertToMeters 0.1;

vertices
(
    (0.0 -0.3 -0.05)		//0
    (3.0 -0.3 -0.05)		//1
    (-0.6 0.0 -0.05)		//2
    (0.0 0.0 -0.05)		//3
    (3.0 0.0 -0.05)		//4
    (-0.6 0.6 -0.05)		//5
    (0.0 0.6 -0.05)		//6
    (3.0 0.6 -0.05)		//7
    (0.0 -0.3 0.05)		//8
    (3.0 -0.3 0.05)		//9
    (-0.6 0.0 0.05)		//10
    (0.0 0.0 0.05)		//11
    (3.0 0.0 0.05)		//12
    (-0.6 0.6 0.05)		//13
    (0.0 0.6 0.05)		//14
    (3.0 0.6 0.05)		//15
);

blocks
(
    hex (2 3 6 5 10 11 14 13) (33 40 1) simpleGrading (0.5 3 1)
    hex (3 4 7 6 11 12 15 14) (100 40 1) simpleGrading (3 3 1)
    hex (0 1 4 3 8 9 12 11) (100 15 1) simpleGrading (3 0.3 1)
);

edges
(
);

boundary
(
    outlet
    {
        type patch;
        faces
        (
            (4 7 15 12)
            (1 4 12 9)
        );
    }
    inlet
    {
        type patch;
        faces
        (
            (2 10 13 5)
        );
    }
    lowerWall
    {
        type wall;
        faces
        (
            (2 3 11 10)
	    (0 8 11 3)
	    (0 1 9 8)
        );
    }
    upperWall
    {
        type wall;
        faces
        (
            (5 13 14 6)
            (6 14 15 7)
        );
    }
);

mergePatchPairs
(
);

// ************************************************************************* //
