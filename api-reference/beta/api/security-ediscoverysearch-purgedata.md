---
title: 'ediscoverySearch: purgeData'
description: Use o método de limpeza de dados para excluir mensagens do Teams em uma pesquisa de Descoberta Eletrônica.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: e61c21c6d4a1238062f550c63d75828eede168e1
ms.sourcegitcommit: 432563e8c81e0f666752445474fe8eada26551e6
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/18/2022
ms.locfileid: "66838371"
---
# <a name="ediscoverysearch-purgedata"></a>ediscoverySearch: purgeData
Namespace: microsoft.graph.security

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Exclua permanentemente as mensagens do Microsoft Teams contidas em [uma pesquisa de Descoberta Eletrônica](../resources/security-ediscoverysearch.md).

>**Nota:** Essa solicitação limpa apenas os dados do Teams. Ele não limpa outros tipos de dados, como itens de caixa de correio.

Você pode coletar e limpar as seguintes categorias de conteúdo do Teams:
- **Chats do Teams 1:1** – mensagens de chat, postagens e anexos compartilhados em uma conversa do Teams entre duas pessoas. Os chats do Teams 1:1 também são chamados *de conversas*.
- **Chats em grupo do Teams** – mensagens de chat, postagens e anexos compartilhados em uma conversa do Teams entre três ou mais pessoas. Também chamado *de chats 1:N* ou conversas *em grupo*.
- **Canais do Teams** – mensagens de chat, postagens, respostas e anexos compartilhados em um canal padrão do Teams.
- **Canais privados** – Postagens de mensagens, respostas e anexos compartilhados em um canal privado do Teams.
- **Canais compartilhados** – Postagens de mensagens, respostas e anexos compartilhados em um canal compartilhado do Teams.

Para obter mais informações sobre como limpar mensagens do Teams, consulte:
- [Série de soluções de Descoberta Eletrônica: cenário de vazamento de dados – Pesquisa e limpeza](/microsoft-365/compliance/data-spillage-scenariosearch-and-purge)
- [Fluxo de trabalho de Descoberta Eletrônica (Premium) para conteúdo no Microsoft Teams](/microsoft-365/compliance/teams-workflow-in-advanced-ediscovery) 


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

# <a name="powershell"></a>[PowerShell](#tab/powershell)
[!INCLUDE [sample-code](../includes/snippets/powershell/ediscoverysearchthispurgedata-powershell-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a>Resposta
Este é um exemplo de resposta.
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
```
