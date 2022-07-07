---
title: Códigos de erro para a API do OneNote no Microsoft Graph
description: Encontre informações sobre códigos de erro retornados pela API do OneNote no Microsoft Graph sempre que uma solicitação enviada por meio da API falhar.
author: jewan-microsoft
ms.localizationpriority: medium
ms.prod: onenote
ms.openlocfilehash: 378dae17b2c0668a33b50a1275f409f9b8e4d015
ms.sourcegitcommit: 7bc623e73fdfb970dbd0a62154d10bb2863afaf7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/07/2022
ms.locfileid: "66668143"
---
# <a name="error-codes-for-the-onenote-api-in-microsoft-graph"></a>Códigos de erro para a API do OneNote no Microsoft Graph

Este artigo descreve os códigos de erro retornados pela API do OneNote no Microsoft Graph sempre que uma solicitação enviada por meio da API falha.

## <a name="error-response-example"></a>Exemplo de resposta de erro

Quando sua solicitação gera um erro, a API do OneNote para de executar a solicitação e retorna uma resposta de erro como um objeto JSON. Uma resposta de erro contém o código de erro associado, uma mensagem e um link para a seção apropriada deste artigo. O exemplo a seguir mostra como é uma resposta de erro.

```json
{
   "error":{
      "code":"10002",
      "message":"The service is currently unavailable. Please try again later.",
      "innerError": {
        "requestId": "request-id",
        "date": "date-time"
      }
   }
}
```

Para saber mais sobre erros do Microsoft Graph, confira [Respostas de erros e tipos de recurso do Microsoft Graph](errors.md).

## <a name="codes-from-10001-to-19999"></a>Códigos de 10001 às 19999

O serviço está tendo problemas ou está enviando informações ao aplicativo.

### <a name="10001"></a>10001
Ocorreu um erro inesperado e a solicitação falhou.

### <a name="10002"></a>10002
O serviço não está disponível no momento.

### <a name="10003"></a>10003
A conta do usuário atual excedeu o número máximo de solicitações ativas. Seu aplicativo terá que repetir a solicitação.

### <a name="10004"></a>10004
O serviço não pode criar uma página na seção solicitada porque essa seção é protegida por uma senha.

### <a name="10005"></a>10005
A solicitação contém mais do que o número máximo de marcas de imagem nas quais o atributo **data-render-src** contém um PDF. Confira [Adicionar imagens e arquivos](onenote-images-files.md).

### <a name="10006"></a>10006
A API do OneNote não pôde criar uma página na seção especificada porque a seção está corrompida.

### <a name="10007"></a>10007
O servidor está ocupado demais para lidar com a solicitação de entrada neste momento. Tente novamente mais tarde.

### <a name="10008"></a>10008
Uma ou mais das bibliotecas de documentos no OneDrive do usuário ou grupo contêm mais de 5.000 itens do OneNote (bloco de anotações, seções, grupos de seções) e não podem ser consultadas usando a API. Certifique-se de que nenhuma das bibliotecas de documentos do grupo ou usuário contenha mais de 5000 itens do OneNote. Confira o [blog de desenvolvimento do OneNote](/archive/blogs/onenotedev/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library) para ver as etapas de mitigação.

### <a name="10012"></a>10012
Não é possível criar nem atualizar a entidade porque a biblioteca que contém o bloco de anotações exige que seja feito check-out dos itens para que eles possam ser editados. Para saber mais, confira [Configurar uma biblioteca para exigir check-out de arquivos](https://support.office.com/article/Configure-a-site-library-to-require-check-out-of-files-f63fcbdc-1db6-4eb7-a3eb-dd815500c9e7).

Remova o requisito de check-out da biblioteca ou mova o bloco de anotações.

### <a name="10013"></a>10013
Uma ou mais das bibliotecas de documentos no OneDrive do usuário ou grupo contêm mais de 20.000 itens e não podem ser indexadas para consulta usando a API. Certifique-se de que nenhuma das bibliotecas de documentos do grupo ou usuário contenha mais de 20.000 itens. Confira o [blog de desenvolvimento do OneNote](/archive/blogs/onenotedev/onenote-api-calls-fail-with-a-large-number-of-items-in-a-sharepoint-document-library) para ver as etapas de mitigação.

### <a name="10014"></a>10014
O Azure Key Vault está ocupado demais para lidar com a solicitação de entrada neste momento. Tente novamente mais tarde.

### <a name="10015"></a>10015
O SharePoint atualmente não está disponível. Tente novamente mais tarde.

### <a name="10016"></a>10016
A biblioteca de documentos no OneDrive do usuário ou grupo excedeu o limite dos escopos exclusivos de segurança. O número máximo de escopos exclusivos de segurança definido para uma biblioteca não pode exceder 50.000.

### <a name="10017"></a>10017
Solicitação Incorreta.

### <a name="19999"></a>19999
A solicitação falhou porque ocorreu um erro indeterminado.

## <a name="codes-from-20001-to-29999"></a>Códigos de 20001 às 29999

O código do aplicativo fez algo errado.

### <a name="20001"></a>20001

A parte "Apresentação" necessária está faltando na solicitação. Exatamente uma é necessária. 

### <a name="20002"></a>20002
A solicitação contém duas ou mais partes de "Apresentação". Exatamente uma é necessária.

### <a name="20003"></a>20003
O tipo de conteúdo da parte "Apresentação" pode ser somente texto/HTML ou aplicativo/XHTML+XML. 

### <a name="20004"></a>20004
O HTML da parte "Apresentação" contém uma marca de imagem com a **src** e o conjunto de propriedades **data-render-src**. A API irá ignorar a propriedade **src** e usar a propriedade **data-render-src**. 

### <a name="20005"></a>20005
O URI da solicitação é muito longo. O tamanho máximo do URI (incluindo todos os parâmetros e dados) é de 16 KB ou 16.384 caracteres.

### <a name="20006"></a>20006
O HTML da parte "Apresentação" contém uma marca de imagem sem a src, nem o conjunto de propriedades **data-render-src**. A API vai ignorar a marca **image**. 

### <a name="20007"></a>20007
O HTML da parte "Apresentação" contém uma cadeia de caracteres de data/hora criada que não corresponde a nenhum dos formatos permitidos. 

### <a name="20008"></a>20008
O tamanho da solicitação é muito grande. 

### <a name="20009"></a>20009
A solicitação contém partes com nomes duplicados. Os nomes das partes devem ser exclusivos. 

### <a name="20010"></a>20010
O cabeçalho Content-Disposition não foi fornecido para o tipo de conteúdo especificado. 

### <a name="20011"></a>20011
A solicitação contém uma carga de partes múltiplas malformadas. Os problemas poderiam incluir ausência de linhas em branco, ausência de uma última linha, separadores de parte formatados incorretamente, etc. Se você estiver criando a mensagem de partes múltiplas à mão, verifique cuidadosamente a lógica, ou considere o uso de uma biblioteca de terceiros. 

### <a name="20012"></a>20012
A solicitação não fornece um tipo de conteúdo para a parte especificada. 

### <a name="20013"></a>20013
A solicitação não fornece cabeçalhos Content-Type e Content-Disposition para a parte especificada. 

### <a name="20014"></a>20014
O comprimento de uma parte na mensagem de partes múltiplas excede o tamanho máximo de 25 MB. 

### <a name="20015"></a>20015
A contagem das partes na mensagem de partes múltiplas excede o limite de 500. 

### <a name="20016"></a>20016
O comprimento da mensagem de partes múltiplas excede o limite de 75 MB. 

### <a name="20017"></a>20017
O MIME do email foi malformado. 

### <a name="20018"></a>20018
O MIME ou ICal da reunião foi malformado. 

### <a name="20019"></a>20019
Nenhum ICal foi encontrado. 

### <a name="20020"></a>20020
Json malformado encontrado no corpo da solicitação. 

### <a name="20100"></a>20100
Algo está errado com a sintaxe da sua solicitação. 

### <a name="20101"></a>20101
A propriedade solicitada não existe.

### <a name="20102"></a>20102
Você solicitou um recurso que não existe.

### <a name="20103"></a>20103
A consulta **expand** não tem suporte para essa solicitação. Confira [Opções de cadeia de caracteres de consulta OData com suporte](onenote-get-content.md#supported-odata-query-string-options).

### <a name="20104"></a>20104
A opção de consulta **pagelevel** tem suporte somente na consulta para a coleção de páginas em uma seção ou para uma página específica. Por exemplo:  

```http
GET ../sections/{id}/pages?pagelevel=true
GET ../pages/{id}?pagelevel=true
```

### <a name="20106"></a>20106
Sua solicitação contém um operador de consulta que não tem suporte. 

### <a name="20108"></a>20108
Sua solicitação contém parâmetros de consulta OData sem suporte.

### <a name="20109"></a>20109
A carga na solicitação PATCH não foi criada corretamente.

### <a name="20110"></a>20110
As solicitações de criação de página com partes de dados exigem que o conteúdo seja de partes múltiplas, com uma parte "Apresentação". 

### <a name="20111"></a>20111
Sua solicitação usa um recurso do OData que não tem suporte.

### <a name="20112"></a>20112
Sua solicitação contém uma ID inválida para o bloco de anotações, o grupo de seções, a seção ou a entidade de página do destino.

### <a name="20113"></a>20113
O recurso especificado na solicitação foi excluído.

### <a name="20115"></a>20115
O nome contém caracteres inválidos. Um nome de bloco de anotações não pode conter nenhum dos seguintes caracteres: `? * \ / : < > | ' "`

### <a name="20117"></a>20117
Um item com o nome especificado já existe no local que você especificou.

### <a name="20119"></a>20119
O HTML na parte "Apresentação" contém um atributo **data-attachment** que não tem um formato válido nem inclui um ou mais desses caracteres inválidos para um nome de arquivo: `\ / : * ? < > | "`. A solicitação substituiu o valor indicado na mensagem de erro.

### <a name="20120"></a>20120
Sua solicitação especifica um destino PATCH que não pode ser localizado.

### <a name="20121"></a>20121
Sua solicitação contém um argumento PATCH inválido. Confira [Atualizar conteúdo da página](onenote-update-page.md).

### <a name="20122"></a>20122
Sua solicitação especifica uma ação PATCH sem suporte. Confira [Atualizar conteúdo da página](onenote-update-page.md).

### <a name="20123"></a>20123
A solicitação PATCH não pode alterar a página especificada.

### <a name="20124"></a>20124
Sua solicitação PATCH de partes múltiplas não inclui uma parte "comandos" com a estrutura JSON da ação PATCH. Confira [Atualizar conteúdo da página](onenote-update-page.md).

### <a name="20125"></a>20125
Sua solicitação PATCH não contém ações. Confira [Atualizar conteúdo da página](onenote-update-page.md).

### <a name="20126"></a>20126
O corpo da mensagem contém JSON incorretamente formatado ou arquivos que não têm suporte para essa operação.

### <a name="20127"></a>20127
Sua solicitação especifica o nome de uma propriedade desconhecida.

### <a name="20128"></a>20128
Sua solicitação contém um erro de sintaxe OData na posição indicada na mensagem.

### <a name="20129"></a>20129
Sua solicitação contém uma opção de cadeia de caracteres de consulta **top** cujo valor é muito alto. Para consultas de página, o valor máximo é 100 e o valor padrão é 20.

### <a name="20130"></a>20130
Sua solicitação contém um URI que aponta para um recurso HTTP que não pode ser encontrado.

### <a name="20131"></a>20131
Sua solicitação contém um valor inválido para Content-Type. Use o valor indicado na mensagem. 

### <a name="20132"></a>20132
Sua solicitação apresentas conteúdo inválido. As causas mais comuns para isso são a ausência do cabeçalho da solicitação Content-Type e/ou nenhum conteúdo no corpo da solicitação. 

### <a name="20133"></a>20133
Sua solicitação especifica um destino PATCH sem suporte. Confira [Atualizar conteúdo da página](onenote-update-page.md).

### <a name="20134"></a>20134
Sua solicitação especifica um elemento inválido como o destino da ação PATCH. Se o destino usar o identificador **data-id**, verifique se ele tem o símbolo # como prefixo. Confira [Atualizar conteúdo da página](onenote-update-page.md).

### <a name="20135"></a>20135
Sua solicitação especifica um tipo de entidade que não tem suporte para a operação PATCH. Confira [Atualizar conteúdo da página](onenote-update-page.md).

### <a name="20136"></a>20136
Sua solicitação contém um atributo **data-render-src** ou **data-render-method** inválido ou que está ausente. Confira [Extrair dados de capturas](onenote-extract-data.md).

### <a name="20137"></a>20137
A página de destino não dá suporte a solicitações PATCH.

### <a name="20138"></a>20138
O tipo de elemento de destino em sua solicitação PATCH não dá suporte à ação **acrescentar**. Confira [Atualizar conteúdo da página](onenote-update-page.md).

### <a name="20139"></a>20139
Sua solicitação contém um valor de atributo **data-tag** inválido. Confira [Usar marcas de anotação](onenote-note-tags.md).

### <a name="20140"></a>20140
Sua solicitação contém um valor de status **data-tag** inválido. A caixa de seleção de marcas de anotação pode ter um status **concluído**. 

Exemplo:

```html
    <p data-tag="to-do:completed">To-do note tag in completed state (checked box in the UI)</p>
```
Confira [Usar marcas de anotação](onenote-note-tags.md).

### <a name="20141"></a>20141
O destino em sua solicitação PATCH não dá suporte à ação especificada. Confira [Atualizar conteúdo da página](onenote-update-page.md).

### <a name="20142"></a>20142
Sua solicitação contém uma expressão **expand** para um pai de entidades filho ou um filho de entidades pai, que não tem suporte. Confira [Opções de cadeia de caracteres de consulta OData com suporte](onenote-get-content.md#supported-odata-query-string-options).

### <a name="20143"></a>20143
A consulta OData é inválida.

### <a name="20144"></a>20144
Sua solicitação contém uma expressão **expand** para uma propriedade de não navegação. Somente as propriedades de navegação podem ser expandidas.

### <a name="20145"></a>20145
A expressão **select** ou **expand** em sua solicitação contém um termo inválido.

### <a name="20146"></a>20146
O atributo `style="position:absolute"`é especificado em um elemento, mas o elemento **body** não especifica `data-absolute-enabled="true"`, que é exigido para dar suporte ao posicionamento. Todas as configurações de posição serão ignoradas. Confira [Criar elementos posicionados absolutos](onenote-abs-pos.md).

### <a name="20147"></a>20147
O atributo `style="position:absolute"` é especificado em um elemento que não é um filho direto do elemento **body**, que não tem suporte. Se o elemento for um **div**, **img** ou **object**, torne-o um filho direto de body; caso contrário, as configurações de posição serão ignoradas e seu conteúdo será renderizado dentro de um div posicionado absoluto. Confira [Criar elementos posicionados absolutos](onenote-abs-pos.md).

### <a name="20148"></a>20148
O atributo `style="position:absolute"` é especificado em um tipo de elemento que não dá suporte a ele. Somente elementos **div**, **img** e **object** que são filhos direto do corpo da página dão suporte ao posicionamento. Confira [Criar elementos posicionados absolutos](onenote-abs-pos.md).

### <a name="20149"></a>20149
Sua solicitação especifica um elemento de destino que não pode ser encontrado.

### <a name="20150"></a>20150
A solicitação não é válida para esse tipo de autenticação. Use o caminho `../me/onenote/` no lugar.

### <a name="20151"></a>20151
A solicitação não é válida para esse tipo de autenticação. Use o ponto de extremidade `../me/onenote/section/{id}/pages` para criar uma página em uma seção específica.

### <a name="20152"></a>20152
Não há qualquer valor de nome especificado para a entidade. O nome deve ser definido e não pode conter somente espaços em branco.

### <a name="20153"></a>20153
O nome da entidade contém caracteres inválidos. O nome não pode conter os seguintes caracteres: `? * \ / : < > | & # " % ~`

### <a name="20154"></a>20154
O nome da entidade não pode começar com um espaço.

### <a name="20155"></a>20155
O nome da entidade é muito longo. Os nomes do bloco de anotações têm um limite de 128 caracteres. Outros nomes de entidade têm um limite de 50 caracteres.

### <a name="20156"></a>20156
A ID especificada para o recurso de destino não existe.

### <a name="20157"></a>20157
A ID especificada para a entidade de destino é inválida.

### <a name="20158"></a>20158
Não é possível obter metadados para a URL do site especificada na solicitação. Verifique o formato da URL fornecida. Os formatos com suporte incluem `https://domain.sharepoint.com/site-a` e `https://domain.com/sites/site-a`.

### <a name="20160"></a>20160
Não é possível encontrar um grupo unificado do Office 365 que tem a ID especificada.

### <a name="20161"></a>20161
O contexto não especifica uma ID de usuário válida. Um erro comum é que PUID/CID foi transmitido como um longo, e não como um hexadecimal.

### <a name="20166"></a>20166
O aplicativo emitiu muitas solicitações em nome de um usuário em um curto período de tempo. Para ajudar a garantir que a API do OneNote permaneça estável e responsiva, a API retorna um código de status 429 e esse erro quando detecta que um aplicativo está usando muitos recursos. 

Para obter mais informações, consulte [as diretrizes](./throttling-limits.md) de limitação específicas do serviço Microsoft Graph.

### <a name="20168"></a>20168
Não há suporte para a fonte do vídeo especificada na solicitação. Confira [Sites de vídeo com suporte](onenote-images-files.md#adding-videos) para a lista atual.


## <a name="codes-from-30001-to-39999"></a>Códigos de 30001 às 39999
Algo está errado com a conta do usuário.

### <a name="30101"></a>30101
A conta do usuário excedeu sua cota do OneDrive. Confira [OneDrive](https://onedrive.live.com/about/).

### <a name="30102"></a>30102
Nada mais pode ser adicionado à seção solicitada porque ela atingiu seu tamanho máximo.

### <a name="30103"></a>30103
O consumo de recursos é muito alto para a solicitação. A conta de usuário de destino tem um grande conjunto de dados ou o serviço está recebendo um grande número de solicitações simultâneas para o mesmo site (por exemplo, o site pessoal do usuário ou um site de equipe).

### <a name="30104"></a>30104
A conta de usuário foi suspensa.

### <a name="30105"></a>30105
O site pessoal do OneDrive for Business do usuário não foi provisionado, que é obrigatório para acessar os blocos de anotações. Agora, o serviço do OneNote provisionará o site. Este processo pode levar algum tempo.

### <a name="30106"></a>30106
O OneDrive for Business está sendo provisionado para o usuário.

### <a name="30108"></a>30108
O OneDrive for Business pessoal do usuário não pôde ser recuperado. A tabela a seguir lista algumas possíveis causas.

| Causa | Resolução |
|:------|:------|
| O site pessoal do usuário não foi provisionado. | O usuário deve abrir o OneDrive for Business e seguir as instruções para provisionar o site. Se isso falhar, eles deverão entrar em contato com o administrador de locatários do Microsoft 365. |
| No momento, o site pessoal do usuário está sendo provisionado. | Tente a solicitação mais tarde. |
| O usuário não tem uma licença válida do OneDrive for Business. | O usuário deve entrar em contato com o administrador de locatários do Microsoft 365. |
| Um problema de rede impediu a solicitação de ser enviada com êxito. | Tente a solicitação mais tarde. |

### <a name="30109"></a>30109
Alguns usuários na solicitação não existem.

### <a name="30110"></a>30110
Os Serviços de Informações do Aluno não foram registrados para esse locatário.

### <a name="30111"></a>30111
Há um erro genérico com os Serviços de Informações do Aluno.

### <a name="30112"></a>30112
Vários usuários afetados pela solicitação tinham o mesmo nome de usuário.

### <a name="30113"></a>30113
O bloco de anotações não está configurado para permitir convites.

### <a name="30114"></a>30114
Há um parâmetro obrigatório ausente.

## <a name="codes-from-40001-to-49999"></a>Códigos de 40001 às 49999
O usuário ou o aplicativo não tem as permissões corretas.

### <a name="40001"></a>40001
A solicitação não contém um token OAuth válido. Confira [Permissões de notas](permissions-reference.md#notes-permissions).

### <a name="40002"></a>40002
O usuário não tem permissão para gravar no local solicitado.

### <a name="40003"></a>40003
O usuário não tem permissão para acessar o recurso solicitado.

### <a name="40004"></a>40004
O token OAuth não tem os escopos necessários para executar a ação solicitada. Confira [Permissões de notas](permissions-reference.md#notes-permissions).

### <a name="40006"></a>40006 
O token OAuth não tem os escopos necessários para executar a ação solicitada. Especificamente a permissão de edição. Confira [Permissões de notas](permissions-reference.md#notes-permissions).

### <a name="40007"></a>40007
O usuário não tem permissões para acessar esse recurso.

### <a name="40008"></a>40008
O acesso é proibido para esse recurso.

### <a name="40009"></a>40009
O contêiner já está em uso por outro recurso.

## <a name="see-also"></a>Confira também

- [Respostas de erro e tipos de recurso do Microsoft Graph](errors.md)
- [Referência da API do OneNote](/graph/api/resources/onenote)
