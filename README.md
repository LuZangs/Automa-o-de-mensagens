# WhatsApp Message Automation Script
Este projeto é um script simples em Python que utiliza Selenium, PyAutoGUI e outras bibliotecas para automatizar o envio de mensagens pelo WhatsApp Web com base em horários pré-definidos.

## Funcionalidades:

Abre o WhatsApp Web automaticamente em horários específicos e envia mensagens predefinidas para números de telefone.
O script fica em execução contínua e verifica o horário a cada 30 segundos para executar as ações no momento certo.
Usa PyAutoGUI para enviar as mensagens após abrir a janela do WhatsApp Web.
Tecnologias Utilizadas


Python: Linguagem de programação utilizada para automação.
Selenium: Para abrir e controlar o navegador.
PyAutoGUI: Para simular a interação com o teclado e enviar as mensagens no WhatsApp Web.
Webbrowser: Para abrir URLs no navegador.
Urllib: Para codificar a mensagem na URL.

## Como Funciona:

O script executa uma verificação contínua do horário usando datetime.now().strftime("%H:%M").
Se o horário atual coincidir com um dos horários predefinidos, o script abre o WhatsApp Web no navegador e preenche automaticamente a mensagem para o número especificado.
Após o envio, o script aguarda 60 segundos antes de continuar ou realizar outras ações.

## Configuração:

Certifique-se de ter o Python instalado.

## Instale as dependências necessárias:

```bash
pip install selenium pyautogui
````

Ajuste os horários, números de telefone e mensagens no código conforme sua necessidade:
```bash
if hora_atual == "14:05":
    telefone = "Numero de telefone"
    mensagem = "Mensagem ou recado"
 ```   
Execução

Execute o script:
```bash
python nome_do_script.py
```
O navegador abrirá automaticamente e enviará as mensagens com base nos horários definidos.
# Uso Consciente
Este código foi projetado para automação de tarefas simples, como envio de lembretes pelo WhatsApp, mas deve ser usado com responsabilidade. Automação de mensagens em massa pode ser vista como uma violação dos termos de uso do WhatsApp. É importante utilizar este script para finalidades legítimas e dentro dos limites éticos.

## Aplicação em Outras Tarefas:
O conceito deste script pode ser expandido para automatizar outras tarefas com base no horário. Aqui estão algumas ideias:

Envio de e-mails automáticos: Você pode adaptar o script para enviar e-mails em horários específicos.

Abertura de páginas da web: Automatize a abertura de sites que você acessa com frequência em horários programados, como portais de estudo ou de trabalho.

Lembretes diários: Além do WhatsApp, use o script para exibir lembretes no seu próprio computador ou para acionar outros aplicativos.

Automação de relatórios: Combine este script com ferramentas de automação de tarefas para gerar relatórios ou backups em horários programados.

Sinta-se à vontade para ajustar e personalizar o código de acordo com suas necessidades.

Observações

O script usa pyautogui.press("Enter") para simular o envio da mensagem no WhatsApp Web.
Certifique-se de que o WhatsApp Web já está configurado no navegador para que o envio ocorra corretamente.
A execução contínua pode ser interrompida pressionando Ctrl + C.

