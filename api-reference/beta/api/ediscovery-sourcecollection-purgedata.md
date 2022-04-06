---
title: 'sourceCollection: purgeData'
description: Use o método purge data para excluir mensagens confidenciais Microsoft Teams extraviadas em uma sourceCollection.
author: mahage-msft
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: a7a2e7ae0138f57739184325b2615d90d74d5abb
ms.sourcegitcommit: 10719607271380ea56076ccff5a3b774d0005773
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/01/2022
ms.locfileid: "64608408"
---
# <a name="sourcecollection-purgedata"></a>sourceCollection: purgeData

Namespace: microsoft.graph.ediscovery

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Exclua permanentemente Microsoft Teams mensagens contidas em [uma sourceCollection](../resources//ediscovery-sourcecollection.md).

>**Observação:** Essa solicitação limpa Teams apenas dados. Ele não limpa outros tipos de dados, como itens de caixa de correio.

Você pode coletar e limpar as seguintes categorias de Teams conteúdo:
- **Teams chats 1:1** - Mensagens de chat, postagens e anexos compartilhados em uma Teams conversa entre duas pessoas. Teams chats 1:1 também são chamados de *conversas*.
- **Teams de grupo** - Mensagens de chat, postagens e anexos compartilhados em uma Teams conversa entre três ou mais pessoas. Também chamado *de chats 1:N* ou conversas *em grupo*.
- **Teams canais** - Mensagens de chat, postagens, respostas e anexos compartilhados em um canal Teams padrão.
- **Canais privados** - Mensagens, respostas e anexos compartilhados em um canal Teams privado.
- **Canais compartilhados** - Mensagens, respostas e anexos compartilhados em um canal Teams compartilhado.

Para obter mais informações sobre como Teams mensagens, consulte:
- [Série de soluções de Descoberta eDiscovery: Cenário de vazamento de dados - Pesquisa e limpeza](/microsoft-365/compliance/data-spillage-scenariosearch-and-purge)
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

Se a operação de limpar dados for iniciada com êxito, essa ação retornará um `202 Accepted` código de resposta. A resposta também conterá um header, que contém o `Location` local da operação [limpar](../resources/ediscovery-purgedataoperation.md) dados que foi criada para confirmação da limpeza.
Para verificar o status da operação de limpeza de dados, faça uma solicitação GET para a URL de local. Quando a solicitação for concluída com êxito, [o status](../resources/ediscovery-caseoperation.md#caseoperationstatus-values) mudará para `succeeded`.

## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
<!-- {
  "blockType": "request",
  "name": "sourcecollectionthis.purgedata"
}
-->
``` http
POST https://graph.microsoft.com/beta/compliance/ediscovery/cases/{caseId}/sourceCollections/{sourceCollectionId}/purgeData
```

### <a name="response"></a>Resposta
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```
