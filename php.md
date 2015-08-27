#PHP

#### OBTENER URL
'''php

$pagina =basename($_SERVER['REQUEST_URI']) ;

	switch ($pagina) {
		case 'catalogo.php':
			echo 'catalogo';
		break;
		
	}

'''
