# OFF098
fn main() {
    let numeros = vec![10,20,30,40,50];
   
    
    for numero in &numeros{
        println!("{}",numero);
    }
}

exercicio 2
fn main() {
    let mut vetor = Vec::new();
    
    
    vetor.push(5);
    vetor.push(10);
    vetor.push(15);
    
    println!("{:?}", vetor); // Deve imprimir[5,10,15]
}

exercicio 3

fn main () {
    let frutas = vec!["maçã", "banana", "laranja"];
    
    
    let primeira = frutas[0];
    let ultima = frutas[frutas.len()-1];
    
    
    println!("Primeira fruta:{}", primeira);
    println!("Última fruta:{}", ultima);
    
}

exercicio 4

fn main() {
    
    let numeros = vec![1,2,3,4,5];
    let tamanho = numeros.len();
    
    
    println!("O vetor tem {} elementos.", tamanho);
}

exercicio 5

fn main() {
    
    let mut vetor = vec![10,20,30];
    vetor.pop(); // Remove o ultimo elemento
    
    println!("{:?}", vetor); // deve imprimir [10,20]
}

//exercicio6

fn main(){
    
    let numeros = vec![1,2,3,4,5];
    let soma: i32 = numeros.iter().sum();
    
    
    println!("A soma dos elementos é :{}", soma);
    
}


//exercicio 7

fn main(){

    let frutas = vec!["maçã","banana","laranja"];
    let procura = "banana";


    if frutas.contains(&procura) {
        println!("{} está no vetor.", procura);
    }
}

// exercicio 8
//fn main (){
  //  let vetor = vec![2;5]; // cria um vetor com 5 elementos, todos iguais a 2


//    println!("{:?}", vetor); // deve imprimir [2,2,2,2,2]
    
//}

// exercicio 9

//fn main(){
    //let frutas = vec!["maçã","banana","laranja"];


   // for (indice,fruta) in frutas.iter().enumerate(){
    //    println!("índice:{},Fruta:{}",indice,fruta);
  //  }
//}

//exercicio 10

fn main(){
    let vetor1 = vec![1,2,3];
    let vetor2 = vec![4,5,6];
    let combinado = [&vetor1[..], &vetor2[..]].concat();

    println!("{:?}", combinado); // deve imprimir [1,2,3,4,5,6]
}

teste 02

//struct Pessoa {
 //    nome: String,
   //   idade:u32,
     // altura:f32,
//}

//fn main(){ 
   
 // let pessoa = Pessoa {
  //  nome: String::from("kaiky"),
   // idade: 28,
   // altura: 1.65,
   // };

//println!("nome:{},idade:{}, altura:{}", pessoa.nome, pessoa.idade, pessoa.altura);
     
 //}



fn main(){
    let pessoa = ("Ana",28,1.65,true);


    let nome = pessoa.0;
    let idade = pessoa.1;
    let altura = pessoa.2;
    let ativo = pessoa.3;
   
    println!("Nome: {},idade:{},altura:{},ativo:{}", nome, idade, altura, ativo);
  
}

//fn main(){
  //  let x = 10;
   // let y= &x;
   // println!("{}",y);
//}

//fn main(){
   // let mut x = 10;
    //let y = &mut x;
   // *y +=1;
  //  println!("{}", y);
//}


fn main(){
    // criando uma pilha usando Vec
    let mut pilha: Vec<&str>=Vec::new();

    // adicionando elementos à pilha (empilhando) 
    pilha.push("joão");
    pilha.push("maria");
    pilha.push("carlos");

    //exibindo a pilha
    println!("Pilha inicial:{:?}", pilha);
    
}


fn main(){
    // criando uma pilha usando Vec
    
    let mut pilha: Vec<&str>=Vec::new();

    // adicionando elementos à pilha (empilhando) 
    
    pilha.push("joão");
    pilha.push("maria");
    pilha.push("carlos");

    //exibindo a pilha
    
    println!("Pilha inicial:{:?}", pilha);

    //removendo elementos da pilha(desempilhamento)

    let topo = pilha.pop();
        println!("topo da pilha:{:?}",topo);
    println!("pilha apos remoçao:{:?}", pilha);

    // adicionando mais elementos
    pilha.push("Ana");
    pilha.push("lucas");
    println!("Pilha após adição:{:?}",pilha);
    //exibindo a pilha após mais inserções
    
    println!("pilha final:{:?}", pilha);
    // removendo mais um elementos
    let topo_2 = pilha.pop();
    
    println!("Novo topo da pilha:{:?}", topo_2);
    println!("pilha final:{:?}", pilha);
}
