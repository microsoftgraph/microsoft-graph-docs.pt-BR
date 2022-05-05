---
title: 'sourceCollection: purgeData'
description: Use o método de limpeza de dados para excluir mensagens confidenciais no Microsoft Teams em uma sourceCollection.
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: fa2bb5cb399d22302d167fd9fb120f13d43e3d43
ms.sourcegitcommit: 4f5a5aef6cfe2fab2ae39ff7eccaf65f44b7aea1
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/05/2022
ms.locfileid: "65211417"
---
# <a name="sourcecollection-purgedata"></a>sourceCollection: purgeData

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Exclua Microsoft Teams mensagens contidas em uma [sourceCollection](../resources//ediscovery-sourcecollection.md).

>**Nota:** Essa solicitação limpa Teams somente dados. Ele não limpa outros tipos de dados, como itens de caixa de correio.

Você pode coletar e limpar as seguintes categorias de Teams conteúdo:
- **Teams chats 1:1** – mensagens de chat, postagens e anexos compartilhados em uma Teams conversa entre duas pessoas. Teams chats 1:1 também são chamados de *conversas*.
- **Teams chats** em grupo – mensagens de chat, postagens e anexos compartilhados em uma Teams conversa entre três ou mais pessoas. Também chamado *de chats 1:N* ou conversas *em grupo*.
- **Teams canais** - mensagens de chat, postagens, respostas e anexos compartilhados em um canal Teams padrão.
- **Canais privados** – Postagens de mensagens, respostas e anexos compartilhados em um canal Teams privado.
- **Canais compartilhados** – Postagens de mensagens, respostas e anexos compartilhados em um canal Teams compartilhado.

Para obter mais informações sobre como limpar Teams mensagens, consulte:
- [Série de soluções de Descoberta Eletrônica: cenário de vazamento de dados – Pesquisa e limpeza](/microsoft-365/compliance/data-spillage-scenariosearch-and-purge)
- [Advanced eDiscovery fluxo de trabalho para conteúdo no Microsoft Teams](/microsoft-365/compliance/teams-workflow-in-advanced-ediscovery) 

## <a name="permissions"></a>Permissions

Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegado (conta corporativa ou de estudante)|eDiscovery.ReadWrite.All|
|Delegado (conta pessoal da Microsoft)|Sem suporte.|
|Aplicativo|Sem suporte.|

## <a name="http-request"></a>Solicitação HTTP

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/purgeData
```

## <a name="request-headers"></a>Cabeçalhos de solicitação

|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação

Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.

Se a operação de limpeza de dados for iniciada com êxito, essa ação retornará um código `202 Accepted` de resposta. A resposta também conterá um cabeçalho, que contém o local da operação [limpar](../resources/ediscovery-purgedataoperation.md) dados que foi criada para confirmar a `Location` limpeza.
Para verificar o status da operação de limpeza de dados, faça uma solicitação GET para a URL de local. Quando a solicitação for concluída com êxito, o [status](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) será alterado para `succeeded`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "sourcecollectionthis.purgedata"
}
-->
``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/purgeData
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/sourcecollectionthispurgedata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/sourcecollectionthispurgedata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[Objective-C](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/sourcecollectionthispurgedata-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/sourcecollectionthispurgedata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/sourcecollectionthispurgedata-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/sourcecollectionthispurgedata-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```
