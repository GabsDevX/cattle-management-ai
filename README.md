# cattle-management-ai
## Funcionalidades
- O arquivo `src/main.py` contém a função principal do software, que atualmente exibe uma mensagem de boas-vindas.

## Tecnologias Utilizadas
- Python
- Flask (para o backend e front-end básico)
- Bibliotecas: `pandas`, `numpy`, `matplotlib`, etc.

## Instalação
1. Clone o repositório:
   ```bash
   git clone https://github.com/GabsDevX/cattle-management-ai.git
   cd cattle-management-ai
   pip install -r requirements.txt
   ```

## Execução
Para evitar problemas de importação, execute o script principal a partir da raiz do projeto usando o seguinte comando:

```bash
python -m src.main
```

Esse comando garante que o Python reconheça o diretório `src/` como um pacote e resolve problemas relacionados ao `PYTHONPATH`.

## Configuração do Front-End
1. Certifique-se de que o Flask está instalado (já incluído no `requirements.txt`).
2. Adicione templates HTML no diretório `templates/` para criar a interface do usuário.
3. Configure rotas no Flask para renderizar as páginas HTML.

## Exemplos de Uso
### Exemplo 1: Visualizar Dados
- Acesse o endpoint `/dados` para visualizar os dados do gado em formato JSON.
- Exemplo de saída:
  ```json
  [
    {"ID": 1, "Peso": 450, "Temperatura": 38.5, "DataColeta": "2023-10-01"},
    {"ID": 2, "Peso": 500, "Temperatura": 39.0, "DataColeta": "2023-10-02"}
  ]
  ```

### Exemplo 2: Análise de Dados
- Acesse o endpoint `/analisar` para obter a média do peso dos animais.
- Exemplo de saída:
  ```json
  {"media_peso": 485.0}
  ```

## Capturas de Tela
### Tela Inicial
![Tela Inicial](screenshots/tela_inicial.png)

### Dados do Gado
![Dados do Gado](screenshots/dados_gado.png)

### Gráficos de Análise
![Gráficos de Análise](screenshots/graficos_analise.png)

## Contribuições
Contribuições são bem-vindas! Siga estes passos para contribuir:
1. Faça um fork do repositório.
2. Crie uma nova branch:
   ```bash
   git checkout -b minha-nova-feature
   ```
3. Faça commit das suas alterações:
   ```bash
   git commit -m "Adiciona nova feature"
   ```
4. Envie para a branch principal:
   ```bash
   git push origin minha-nova-feature
   ```
5. Abra um Pull Request.

## Licença
Este projeto está licenciado sob a licença MIT.

