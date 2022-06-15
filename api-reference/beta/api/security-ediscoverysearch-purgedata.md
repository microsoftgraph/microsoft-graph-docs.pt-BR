---
title: 'ediscoverySearch: purgeData'
description: Use o método de limpar dados para excluir Teams mensagens em uma pesquisa de Descoberta Eletrônica.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: f8ac399b59473a4c5ec1d1e1f064532228c23ea5
ms.sourcegitcommit: 6bb3c5c043d35476e41ef2790bcf4813fae0769d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/15/2022
ms.locfileid: "66095388"
---
# <a name="ediscoverysearch-purgedata"></a>ediscoverySearch: purgeData
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Exclua Microsoft Teams mensagens contidas em [uma pesquisa de Descoberta Eletrônica](../resources/security-ediscoverysearch.md).

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


## <a name="permissions"></a>Permissões
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
POST /security/cases/ediscoveryCases/{ediscoveryCaseId}/searches/{ediscoverySearchId}/purgeData
```

## <a name="request-headers"></a>Cabeçalhos de solicitação
|Nome|Descrição|
|:---|:---|
|Autorização|{token} de portador. Obrigatório.|

## <a name="request-body"></a>Corpo da solicitação
Não forneça um corpo de solicitação para esse método.

## <a name="response"></a>Resposta

Se tiver êxito, esta ação retornará um código de resposta `202 Accepted`.

Se a operação de limpeza de dados for iniciada com êxito, essa ação retornará um código `202 Accepted` de resposta. A resposta também conterá um cabeçalho, que contém o local da operação [limpar](../resources/security-ediscoverypurgedataoperation.md) dados que foi criada para confirmar a `Location` limpeza.
Para verificar o status da operação de limpeza de dados, faça uma solicitação GET para a URL de local.


## <a name="examples"></a>Exemplos

### <a name="request"></a>Solicitação
Veja a seguir um exemplo de uma solicitação.

# <a name="http"></a>[HTTP](#tab/http)
<!-- {
  "blockType": "request",
  "name": "ediscoverysearchthis.purgedata"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/searches/c61a5860-d634-4d14-aea7-d82b6f4eb7af/purgeData
```
# <a name="c"></a>[C#](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/ediscoverysearchthispurgedata-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[JavaScript](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/ediscoverysearchthispurgedata-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[Java](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/ediscoverysearchthispurgedata-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="go"></a>[Ir](#tab/go)
[!INCLUDE [sample-code](../includes/snippets/go/ediscoverysearchthispurgedata-go-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
A seguir está um exemplo da resposta
>**Observação:** o objeto de resposta mostrado aqui pode ser encurtado para legibilidade.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```
