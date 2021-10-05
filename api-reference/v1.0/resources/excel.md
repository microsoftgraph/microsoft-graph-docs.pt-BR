---
title: Trabalhando com o Excel no Microsoft Graph
description: O Microsoft Graph pode ser usado para permitir que aplicativos Web e dispositivos móveis leiam e modifiquem as pastas de trabalho do Excel armazenadas no OneDrive for Business, site do SharePoint ou Group drive.
ms.localizationpriority: high
author: grangery
ms.prod: excel
doc_type: conceptualPageType
ms.openlocfilehash: cf035bc3d9cef6442a220bc14de6f9a0c81f589a
ms.sourcegitcommit: 94dc71a6d4fbdc46f2681a1add13416bc9b4a6e9
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/05/2021
ms.locfileid: "60115148"
---
# <a name="working-with-excel-in-microsoft-graph"></a>Trabalhando com o Excel no Microsoft Graph

É possível usar o Microsoft Graph para permitir que aplicativos Web e móveis leiam e modifiquem pastas de trabalho do Excel armazenadas no OneDrive for Business, site do SharePoint ou unidade do Grupo. O recurso `Workbook` (ou arquivo do Excel) contém todos os outros recursos do Excel por meio de relações. É possível acessar uma pasta de trabalho por meio da [API Drive](drive.md) identificando a localização do arquivo na URL. Por exemplo:

`https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/`  
`https://graph.microsoft.com/v1.0/me/drive/root:/{item-path}:/workbook/`  

Você pode acessar um conjunto de objetos do Excel (como Table, Range ou Chart) usando APIs REST padrão para realizar operações de criação, leitura, atualização e exclusão (CRUD) na pasta de trabalho. Por exemplo, `GET https://graph.microsoft.com/v1.0/me/drive/items/{id}/workbook/worksheets`  
retorna uma coleção de todos os objetos da planilha que fazem parte da pasta de trabalho.    


A API REST do Excel só oferece suporte para pastas de trabalho formatadas pelo arquivo do Office Open XML. Não há suporte para pastas de trabalho de extensão de `.xls`. 

**Observação**: o suporte para pastas de trabalho armazenadas na plataforma de Consumidor do OneDrive ainda não está disponível. Neste momento, somente os arquivos armazenados em plataformas comerciais têm suporte das APIs REST do Excel. 

## <a name="authorization-and-scopes"></a>Autorização e escopos

Você pode usar o [ponto de extremidade do Microsoft Azure AD v.2](/graph/auth-register-app-v2) para autenticar as APIs do Excel. Todas as APIs exigem o cabeçalho HTTP `Authorization: Bearer {access-token}`.   
  
Um dos seguintes [escopos de permissão](/graph/permissions-reference) é obrigatório para usar o recurso do Excel:

* Files.Read (para ações de leitura)
* Files.ReadWrite (para ações de leitura e gravação)


## <a name="sessions-and-persistence"></a>Sessões e persistência

As APIs do Excel podem ser chamadas em um destes três modos: 

1. Sessão persistente - Todas as alterações feitas na pasta de trabalho são persistentes (salvas). Este é o modo de operação mais eficiente e com o desempenho mais elevado. 
2. Sessão não persistente – As alterações feitas pela API não são salvas na localização de origem. Em vez disso, o servidor back-end do Excel mantém uma cópia temporária do arquivo que reflete as alterações feitas durante essa sessão de API específica. Quando a sessão do Excel expirar, as alterações serão perdidas. Esse modo é útil para aplicativos que precisam fazer uma análise ou obter os resultados de um cálculo ou de uma imagem de gráfico, mas não afeta o estado do documento. 
3. Sem sessão ‒ a chamada à API é feita sem informações sobre a sessão. Os servidores do Excel têm que localizar a cópia do servidor de pasta de trabalho sempre que executam a operação. Portanto, essa não é uma maneira eficiente de chamar APIs do Excel. Ele é adequado para fazer solicitações únicas. 

Para representar a sessão na API, use o cabeçalho `workbook-session-id: {session-id}`. 

>**Observação:** o cabeçalho de sessão não é obrigatório para uma API do Excel funcionar. No entanto, recomendamos que você use o cabeçalho de sessão para melhorar o desempenho. Se você não usar um cabeçalho de sessão, as alterações feitas durante a chamada à API _serão_ mantidas como persistentes no arquivo.  

### <a name="api-call-to-get-a-session"></a>Chamada à API para obter uma sessão 

#### <a name="request"></a>Solicitação 

Passe um objeto JSON definindo o valor de `persistchanges` como `true` ou `false`. 

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/createSession
content-type: Application/Json 
authorization: Bearer {access-token}

{ "persistChanges": true }
```

Quando o valor de `persistChanges` está definido como `false`, uma id de sessão não persistente é retornada.  


#### <a name="response"></a>Resposta

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#microsoft.graph.sessionInfo",
  "id": "{session-id}",
  "persistChanges": true
}
```

#### <a name="usage"></a>Uso 

A ID de sessão retornada da chamada anterior é transmitida como um cabeçalho em solicitações de API subsequentes no  
cabeçalho HTTP `workbook-session-id`. 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

>Observação: se a id da sessão tiver expirado, um código de erro HTTP `404` será retornado na sessão. Nesse cenário, você pode optar por criar uma nova sessão e continuar. Outra abordagem seria atualizar a sessão periodicamente para manter a sessão ativa. Geralmente, a sessão persistente expira após cerca de 5 minutos de inatividade. A sessão não persistente expira após cerca de 7 minutos de inatividade. 

## <a name="common-excel-scenarios"></a>Cenários comuns do Excel

Esta seção fornece exemplos das operações comuns que você pode usar em objetos do Excel.

### <a name="worksheet-operations"></a>Operações de planilha

#### <a name="list-worksheets-part-of-the-workbook"></a>Listar a parte de planilhas da pasta de trabalho 
Solicitação 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

Resposta

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)",
      "id": "{00000000-0001-0000-0000-000000000000}",
      "name": "Sheet1",
      "position": 0,
      "visibility": "Visible"
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B00000000-0001-0000-0100-000000000000%7D%27)",
      "id": "{00000000-0001-0000-0100-000000000000}",
      "name": "Sheet57664",
      "position": 1,
      "visibility": "Visible"
    }
  ]
}
```
#### <a name="add-a-new-worksheet"></a>Adicionar uma nova planilha 
 
<!-- { "blockType": "ignored" } -->
```http
POST /{version}/me/drive/root:/workbook/worksheets
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "Sheet32243" }
```

Resposta
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/{version}/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D%27)",
  "id": "{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}",
  "name": "Sheet32243",
  "position": 5,
  "visibility": "Visible"
}
```

#### <a name="get-a-new-worksheet"></a>Obter uma nova planilha 

Obter uma planilha com base no nome. 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets/Sheet32243
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

Resposta
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D%27)",
  "id": "{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}",
  "name": "Sheet32243",
  "position": 5,
  "visibility": "Visible"
}
```

** Observação: as planilhas também podem ser recuperadas usando a ID. No entanto, atualmente, a ID contém os caracteres `{` e '}' que precisam ser codificados pela URL para a API funcionar. Exemplo: Para obter uma planilha com a ID de `{75A18F35-34AA-4F44-97CC-FDC3C05D9F40}`, a URL codifica a ID no caminho como `/workbook/worksheets/%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D`. 

#### <a name="delete-a-worksheet"></a>Excluir uma planilha

Solicitação
```
DELETE https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('%7B75A18F35-34AA-4F44-97CC-FDC3C05D9F40%7D')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

Resposta
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```


#### <a name="update-worksheet-properties"></a>Atualizar as propriedades da planilha

Solicitação 

```
PATCH https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets/SheetA
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "SheetA", "position": 3 }
```

Resposta

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN')/workbook/worksheets(%27%7B00000000-0001-0000-0100-000000000000%7D%27)",
  "id": "{00000000-0001-0000-0100-000000000000}",
  "name": "SheetA",
  "position": 3,
  "visibility": "Visible"
}
```

### <a name="chart-operations"></a>Operações de gráfico

#### <a name="list-charts-that-are-part-of-the-worksheet"></a>Listar gráficos que fazem parte da planilha 

Solicitação
<!-- { "blockType": "ignored" } -->
```http 
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id} 
```

Resposta
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)/charts(%27%7B00000000-0008-0000-0100-000003000000%7D%27)",
      "height": 235.5,
      "id": "{00000000-0008-0000-0100-000003000000}",
      "left": 276.0,
      "name": "Chart 2",
      "top": 0.0,
      "width": 401.25
   }
  ]
}
```

** Observação: a ID contém os caracteres `{` e `}` (exemplo: `{00000000-0008-0000-0100-000003000000}`) que precisam ser codificados pela URL para a API funcionar. Exemplo: Para obter um objeto gráfico, a URL codifica a ID no caminho como `/charts/%7B00000000-0008-0000-0100-000003000000%7D`. 

#### <a name="get-chart-image"></a>Obter imagem do gráfico

Solicitação
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B00000000-0008-0000-0100-000003000000%7D')/Image(width=0,height=0,fittingMode='fit')
authorization: Bearer {access-token} 
workbook-session-id: {session-id} 
```

Resposta
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Edm.String",
  "value": "{base-64-string}"
}
```

#### <a name="add-a-chart"></a>Adicionar um gráfico  

Solicitação

<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts/Add
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 

{ "type": "ColumnClustered", "sourcedata": "A1:C4", "seriesby": "Auto" }
```

Resposta
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#chart",
  "@odata.type": "#microsoft.graph.workbookChart",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)/charts(%27%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D%27)",
  "height": 216.0,
  "id": "{2D421098-FA19-41F7-8528-EE7B00E4BB42}",
  "left": 0.0,
  "name": "Chart 2",
  "top": 0.0,
  "width": 360.0
}
```

#### <a name="update-a-chart"></a>Atualizar um gráfico

<!-- { "blockType": "ignored" } -->
```http 
PATCH https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "height": 216.0, "left": 0, "name": "NewName", "top": 0, "width": 360.0 }

```
Resposta 

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL')/workbook/worksheets(%27%7B00000000-0001-0000-0000-000000000000%7D%27)/charts(%27%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D%27)",
  "height": 216.0,
  "id": "{2D421098-FA19-41F7-8528-EE7B00E4BB42}",
  "left": 0.0,
  "name": "NewName",
  "top": 0.0,
  "width": 360.0
}
```

#### <a name="update-chart-source-data"></a>Atualizar dados de origem do gráfico 

Solicitação
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/charts('%7B2D421098-FA19-41F7-8528-EE7B00E4BB42%7D')/setData
content-type: Application/Json 
accept: application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "sourceData": "A1:C4", "seriesBy": "Auto" }
```

Resposta
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

### <a name="table-operations"></a>Operações de tabela 

#### <a name="get-list-of-tables"></a>Obter lista de tabelas 

Solicitação
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJB6K563VVUU2ZC2FJBAHLSZZQXL/workbook/worksheets('%7B00000000-0001-0000-0000-000000000000%7D')/tables
accept: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

Resposta
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 
```

#### <a name="create-table"></a>Criar tabela

Solicitação
<!-- { "blockType": "ignored" } -->
```http 
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables/{table-id}/add
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "NewTableName", "hasHeaders": true, "showTotals": false, "style": "TableStyleMedium4" }
```

Resposta
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%272%27)",
  "id": "2",
  "name": "NewTableName",
  "showHeaders": true,
  "showTotals": false,
  "style": "TableStyleMedium4"
}
```

#### <a name="update-table"></a>Atualizar tabela

Solicitação
<!-- { "blockType": "ignored" } -->
```http 
PATCH https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('2')
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "name": "NewTableName", "showHeaders": true, "showTotals": false, "style": "TableStyleMedium4" }
```

Resposta
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%272%27)",
  "id": "2",
  "name": "NewTableName",
  "showHeaders": true,
  "showTotals": false,
  "style": "TableStyleMedium4"
}
```

#### <a name="get-list-of-table-rows"></a>Obter lista de linhas de tabelas
Solicitação 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/rows
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

Resposta

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('4')/rows",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(0)",
      "index": 0,
      "values": [
        [
          42019,
          53,
          34
       ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(1)",
      "index": 1,
      "values": [
        [
          42020,
          45,
          39
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(2)",
      "index": 2,
      "values": [
        [
          42021,
          50,
          31
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(3)",
      "index": 3,
      "values": [
        [
          42022,
          43,
          39
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(4)",
      "index": 4,
      "values": [
        [
          42023,
          45,
          41
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows/itemAt(5)",
      "index": 5,
      "values": [
        [
          42024,
          52,
          40
        ]
      ]
    }
  ]
}
```

#### <a name="get-list-of-table-columns"></a>Obter lista de colunas de tabelas

Solicitação
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/columns
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

Resposta 

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK 
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('4')/columns",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/columns(%271%27)",
      "id": "1",
      "index": 0,
      "name": "Date",
      "values": [
        [
          "Date"
        ],
        [
          42019
       ],
        [
          42020
        ],
        [
          42021
        ],
        [
          42022
        ],
        [
          42023
        ],
        [
          42024
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/columns(%272%27)",
      "id": "2",
      "index": 1,
      "name": "High (F)",
      "values": [
        [
          "High (F)"
        ],
        [
          53
        ],
        [
          45
        ],
        [
          50
        ],
        [
          43
        ],
        [
          45
        ],
        [
          52
        ]
      ]
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/columns(%273%27)",
      "id": "3",
      "index": 2,
      "name": "Low (F)",
      "values": [
        [
          "Low (F)"
        ],
        [
          34
        ],
        [
          39
        ],
        [
          31
        ],
        [
          39
        ],
        [
          41
        ],
        [
          40
        ]
      ]
    }
  ]
}
```


#### <a name="add-a-table-row"></a>Adicionar uma linha de tabela

Solicitação
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/rows
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "values": [ [ "Jan-15-2016", "49", "37" ] ], "index": null }
```

Resposta
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('4')/rows/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%274%27)/rows(null)",
  "index": 6,
  "values": [
    [
      "Jan-15-2016",
      49,
      37
    ]
  ]
}
```

#### <a name="add-a-table-column"></a>Adicionar uma coluna de tabela 

Solicitação
<!-- { "blockType": "ignored" } -->
```http 
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('2')/columns
content-type: Application/Json 
accept: application/Json 


{ "values": [ [ "Status" ], [ "Open" ], [ "Closed" ] ], "index": 2 }
```

Resposta 

<!-- { "blockType": "ignored" } -->
```http 
HTTP code: 201 Created
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables('2')/columns/$entity",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/tables(%272%27)/columns(%274%27)",
  "id": "4",
  "index": 2,
  "name": "Status",
  "values": [
    [
      "Status"
    ],
    [
      "Open"
    ],
    [
      "Closed"
    ]
  ]
}
```

#### <a name="delete-table-row"></a>Excluir linha de tabela

Solicitação
<!-- { "blockType": "ignored" } -->
```http  
DELETE https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/rows/$/itemAt(index=6)
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

Resposta
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

#### <a name="delete-table-column"></a>Excluir coluna de tabela 
Solicitação
<!-- { "blockType": "ignored" } -->
```http
DELETE https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('4')/columns('3')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

Resposta
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

#### <a name="convert-table-to-range"></a>Converter tabela em intervalo 
Solicitação
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/tables('1')/convertToRange
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

Resposta
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK 
content-type: application/json;odata.metadata 
```

#### <a name="table-sort"></a>Classificação de tabela
Solicitação
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/tables('table2')/sort/apply
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"fields" : [
  { "key": 0,
   "ascending": true
  }
]
}
```


Resposta
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

#### <a name="table-filter"></a>Filtro de tabela
Solicitação
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/tables('table2')/columns(id='2')/filter/apply
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"criteria" : 
  { "filterOn": "custom",
   "criterion1": ">15",
   "operator": "and",
   "criterion2": "<50"
   
  }
}
```

Resposta
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```


#### <a name="clear-filter"></a>Limpar filtro
Solicitação
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/tables('table2')/columns(id='2')/filter/clear
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

Resposta
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```

### <a name="range-operations"></a>Operações de intervalo

#### <a name="get-range"></a>Obter intervalo 

Solicitação
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/{item-id}/workbook/worksheets/{worksheet-id}/range(address='A1:B2')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

Resposta 

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata 

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#range",
  "@odata.type": "#microsoft.graph.workbookRange",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/worksheets(%27%7B00000000-0001-0000-0300-000000000000%7D%27)/range(address=%27A1:B2%27)",
  "address": "test!A1:B2",
  "addressLocal": "test!A1:B2",
  "cellCount": 4,
  "columnCount": 2,
  "columnHidden": false,
  "columnIndex": 0,
  "formulas": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "formulasLocal": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "formulasR1C1": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "hidden": false,
  "numberFormat": [
    [
      "General",
      "General"
    ],
    [
      "General",
      "General"
    ]
  ],
  "rowCount": 2,
  "rowHidden": false,
  "rowIndex": 0,
  "text": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "values": [
    [
      "",
      ""
    ],
    [
      "",
      ""
    ]
  ],
  "valueTypes": [
    [
      "Empty",
      "Empty"
    ],
    [
      "Empty",
      "Empty"
    ]
  ]
}
```

#### <a name="range-update"></a>Atualização de intervalo 

<!-- { "blockType": "ignored" } -->
```http
PATCH https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/worksheets('test')/range(address='test!A1:B2')
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{ "values": [ [ "Test", "Value" ], [ "For", "Update" ] ] }
```

<!-- { "blockType": "ignored" } -->
```http
HTTP code: 200 OK
content-type: application/json;odata.metadata

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#range",
  "@odata.type": "#microsoft.graph.workbookRange",
  "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/worksheets(%27%7B00000000-0001-0000-0300-000000000000%7D%27)/range(address=%27test!A1:B2%27)",
  "address": "test!A1:B2",
  "addressLocal": "test!A1:B2",
  "cellCount": 4,
  "columnCount": 2,
  "columnHidden": false,
  "columnIndex": 0,
  "formulas": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "formulasLocal": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "formulasR1C1": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "hidden": false,
  "numberFormat": [
    [
      "General",
      "General"
    ],
    [
      "General",
      "General"
    ]
  ],
  "rowCount": 2,
  "rowHidden": false,
  "rowIndex": 0,
  "text": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "values": [
    [
      "Test",
      "Value"
    ],
    [
      "For",
      "Update"
    ]
  ],
  "valueTypes": [
    [
      "String",
      "String"
    ],
    [
      "String",
      "String"
    ]
  ]
}
```

#### <a name="range-sort"></a>Classificação de intervalo
Solicitação
<!-- { "blockType": "ignored" } -->
```http
POST https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJGUJ7JHBSZDFZFL25KSZGQTVAUN/workbook/worksheets('Sheet15799')/usedRange/sort/apply
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
"fields" : [
  { "key": 0,
   "ascending": true
  }
]
}
```

Resposta
<!-- { "blockType": "ignored" } -->
```http
HTTP code: 204 No Content
```


### <a name="named-items"></a>Itens nomeados
Solicitação

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/v1.0/me/drive/items/01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4/workbook/names
authorization: Bearer {access-token} 
workbook-session-id: {session-id}
```

Resposta 

<!-- { "blockType": "ignored" } -->
```http 
HTTP code: 200 OK
content-type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names",
  "value": [
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names(%27data%27)",
      "name": "data",
      "type": "Range",
      "value": "Range!$A$1:$D$3",
      "visible": true
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names(%27myrange%27)",
      "name": "myrange",
      "type": "Range",
      "value": "Range!$E$1:$F$7",
      "visible": true
    },
    {
      "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/items('01CYZLFJDYBLIGAE7G5FE3I4VO2XP7BLU4')/workbook/names(%27range1%27)",
      "name": "range1",
      "type": "Range",
      "value": "Range!$I$1:$M$11",
      "visible": true
    }
  ]
}
```

### <a name="work-with-nulls"></a>Trabalhar com nulos

#### <a name="null-input-in-2-d-array"></a>entrada nula em uma matriz 2D

A entrada `null` em uma matriz bidimensional (para valores, formato de número ou fórmula) é ignorada nos recursos Range e Table. Nenhuma atualização será realizada no destino pretendido (célula) quando a entrada `null` for enviada em valores, formato de número ou grade de fórmula de valores.

Por exemplo, para atualizar somente partes específicas de Range, como o formato de número de uma célula, e para manter o formato de número existente em outras partes de Range, defina o formato de número onde for obrigatório e envie `null` para as outras células.

Na solicitação de definição a seguir, somente algumas partes do formato de número de Range são definidas, enquanto o formato de número existente na parte restante é mantido (por meio da transmissão de nulos).

```json
{
  "values" : [["Eurasia", "29.96", "0.25", "15-Feb" ]],
  "numberFormat" : [[null, null, null, "m/d/yyyy;@"]]
}
```

#### <a name="null-input-for-a-property"></a>entrada nula para uma propriedade

`null` não é uma entrada válida única para toda a propriedade. Por exemplo, o modelo a seguir não é válido, uma vez que os valores inteiros não podem ser ignorados ou definidos como nulos.

```json
{
"values":  null
}

```

O exemplo a seguir também não é válido, porque nulo não é um valor de cor válido.

```json
{
"color" :  null
}
```

#### <a name="null-response"></a>Resposta nula

Representação de propriedades de formatação que consiste em valores não uniformes que resultam no retorno de um valor nulo na resposta.

Por exemplo, um intervalo pode consistir em uma ou mais células. Nos casos em que as células individuais incluídas no intervalo especificado não apresentam valores de formatação uniformes, a representação de nível do intervalo será indefinida.

```json
{
  "size: : null,
  "color" : null
}
```

Um valor nulo também é retornado na resposta nos seguintes casos:
- Se ocorrer um erro ao tentar obter uma determinada propriedade de um objeto e essa propriedade puder ser definida como nula, a propriedade pode retornar um valor nulo na resposta.
- Para um objeto Range, ao obter um intervalo para linha inteira ou coluna inteira, algumas propriedades podem retornar nulo como a resposta. Se o tamanho do intervalo exceder a limitação superior (células 5M), algumas propriedades retornarão nulas como o valor.

### <a name="blank-input-and-output"></a>Entrada e saída em branco

Valores em branco em solicitações de atualização são tratados como uma instrução para limpar ou redefinir a respectiva propriedade. Um valor em branco é representado por aspas duplas sem espaço entre elas: `""`

Exemplos:

* Para `values`, o valor do intervalo é removido. Isso equivale a limpar o conteúdo do aplicativo.

* Para `numberFormat`, o formato de número é definido como `General`.

* Para `formula` e `formulaLocale`, os valores de fórmula são excluídos.


Para operações de leitura, espera-se receber valores em branco caso o conteúdo das células esteja em branco. Quando a célula não inclui dados ou valores, a API retorna um valor em branco. O valor em branco é representado por aspas duplas sem espaço entre elas: `""`

```json
{
  "values" : [["", "some", "data", "in", "other", "cells", ""]]
}
```

```json
{
  "formula" : [["", "", "=Rand()"]]
}
```


### <a name="unbounded-range"></a>Intervalo não associado

#### <a name="read"></a>Leitura

Um endereço de intervalo não associado contém apenas os identificadores de coluna ou de linha e identificador não especificado de linha ou de coluna, respectivamente, como:

* `C:C`, `A:F`, `A:XFD` (inclui linhas não especificadas)
* `2:2`, `1:4`, `1:1048546` (inclui colunas não especificadas)

Quando a API faz uma solicitação para recuperar um intervalo não associado (`getRange('C:C')`), a resposta retornada contém `null` para as propriedades em nível de célula, como `values`, `text`, `numberFormat` ou `formula`. Outras propriedades de Range, como `address` ou `cellCount`, refletirão o intervalo não associado.

#### <a name="write"></a>Gravação

O sistema **não permite** a definição de propriedades de nível da célula (como values, numberFormat, etc.) em um intervalo não associado, pois a solicitação de entrada pode ser muito extensa para ser manipulada.

O exemplo a seguir não é uma solicitação de atualização válida, pois o intervalo solicitado não está associado.

<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/root/workbook/worksheets/{id}/range(address="A:B")

{
  "values" : "Due Date"
}
```

Quando uma operação de atualização é tentada nesse intervalo, a API retorna um erro.


### <a name="large-range"></a>Intervalo longo

Um intervalo longo significa um intervalo cujo tamanho é muito grande para uma única chamada à API. Muitos fatores, como o número de células, os valores, os formatos de número e as fórmulas incluídas no intervalo, podem fazer com que a resposta seja tão extensa a ponto de se tornar inadequada para interação com a API. A API faz a melhor tentativa para retornar ou gravar os dados solicitados. No entanto, o tamanho extenso envolvido pode resultar em uma condição de erro da API devido à intensa utilização de recursos.

Para evitar isso, convém fazer leituras ou gravações para um intervalo longo em vários tamanhos de intervalo menores.


### <a name="single-input-copy"></a>Cópia de entrada única

Para dar suporte a atualização de um intervalo com os formatos de número ou valores idênticos, ou para a aplicação de uma mesma fórmula em um intervalo, você deve usar a seguinte convenção na API de configuração. No Excel, esse comportamento é semelhante a inserir valores ou fórmulas em um intervalo no modo Ctrl+Enter.

A API vai procurar um *valor de célula única*, no entanto, se a dimensão do intervalo de destino não corresponder à dimensão do intervalo de entrada, ela aplicará a atualização ao intervalo inteiro no modo Ctrl+Enter com o valor ou fórmula fornecida na solicitação.

#### <a name="examples"></a>Exemplos

A solicitação a seguir atualiza o intervalo selecionado com "Texto de amostra". Observe que o intervalo tem 200 células, ao passo que a entrada fornecida tem apenas 1 valor de célula.

<!-- { "blockType": "ignored" } -->
```http
PATCH /me/drive/root/workbook/worksheets/{id}/range(address="A1:B100")

{
  "values" : "Sample text"
}
```

### <a name="workbook-functions"></a>Funções de pasta de trabalho 
Você pode acessar as funções de pasta de trabalho por meio de uma coleção de funções incluídas no recurso /Functions. 

<!-- LG: Where is the Functions resource? We should link to this.
-->
##### <a name="request"></a>Solicitação
<!-- { "blockType": "ignored" } -->
```http
https://graph.microsoft.com/v1.0/me/drive/root:/book1.xlsx:/workbook/functions/pmt
content-type: Application/Json 
authorization: Bearer {access-token} 
workbook-session-id: {session-id}

{
    "rate": 4.5,
    "nper": 12,
    "pv": -1250
}
```


##### <a name="response"></a>Resposta 

<!-- { "blockType": "ignored" } -->
```http 
HTTP code: 200 OK
content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#workbookFunctionResult",
    "@odata.type": "#microsoft.graph.workbookFunctionResult",
    "@odata.id": "/users('f6d92604-4b76-4b70-9a4c-93dfbcc054d5')/drive/root/workbook/functions/pmt()",
    "error": null,
    "value": 5625.00000734125
}
```

## <a name="error-information"></a>Informações do erro 

Erros são retornados com um código de erro HTTP e um objeto de erro. Um `code` de erro e uma `message` explicam o motivo do erro.
 
Apresentamos um exemplo a seguir.

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 400 Bad Request
Content-Type: application/json

{
  "error": {
    "code": "ItemAlreadyExists",
    "message": "A resource with the same name or identifier already exists.",
    "innerError": {
      "request-id": "214ca7ea-9ea4-442e-9c67-71fdda0a559c",
      "date": "2016-07-28T03:56:09"
    }
  }
}
```

## <a name="whats-new"></a>Novidades
Saiba mais sobre os [novos recursos e atualizações mais recentes](/graph/whats-new-overview) para este conjunto de APIs.
