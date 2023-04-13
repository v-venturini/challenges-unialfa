 <html lang="en">
 <head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
   <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
 <title>Produtos de Mercado</title>
 </head>
 <body>
    <h2>MERCADO DA VI</h2>
    <table>
        <tr>
            <th>Produto</th>
            <th>Marca</th>
            <th>Preço</th>
        </tr>
        
 <?php 

        require('produtos.php');
        foreach($produtos as $produto) {
            echo "<tr>";
            echo "<td>" . $produto['produto'] . "</td>";
            echo "<td>" . $produto['marca'] . "</td>";
            echo "<td>" . $produto['preco'] . "</td>";
            echo "</tr>";
        }           
 ?>
    </table>    
 </body>
 </html>

<?php 

    
$produtos = [
    [
    "produto" => "Arroz",
    "marca" => "Tio João",
    "preco" => 28.49, 
    ],
    [
    "produto" => "Feijão",
    "marca" => "Kicaldo",
    "preco" => 12.99, 
    ],
    [
    "produto" => "Carne",
    "marca" => "Friboi",
    "preco" => 32.99, 
    ],
    [
    "produto" => "Leite",
    "marca" => "Piracanjuba",
    "preco" => 4.89, 
    ],
    [
    "produto" => "Pão",
    "marca" => "Wickbold",
    "preco" => 7.89,
    ],
    [
    "produto" => "Ovos",
    "marca" => "Granja Milena",
    "preco" => 7.49, 
    ],
    [
    "produto" => "Manteiga",
    "marca" => "Qualy",
    "preco" => 11.99, 
    ],
    [
    "produto" => "Açucar",
    "marca" => "União",
    "preco" => 12.90, 
    ],
    [
    "produto" => "Café",
    "marca" => "Tres Corações",
    "preco" => 13.99, 
    ],
    [
    "produto" => "Banana",
    "marca" => "Maça",
    "preco" => 6.49, 
    ],
]; 

?>