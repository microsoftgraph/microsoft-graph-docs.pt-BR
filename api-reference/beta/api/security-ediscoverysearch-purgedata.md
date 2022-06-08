---
title: 'ediscoverySearch: purgeData'
description: Use o método de limpeza de dados para excluir mensagens do Teams em uma pesquisa de Descoberta Eletrônica.
author: SeunginLyu
ms.localizationpriority: medium
ms.prod: ediscovery
doc_type: apiPageType
ms.openlocfilehash: 316e7d673b9810b7fdfac655f387e192bc958c84
ms.sourcegitcommit: a345f96fb22115f65840702a4acf0acc7c1b0679
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/08/2022
ms.locfileid: "65945128"
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
- [Fluxo de trabalho de Descoberta Eletrônica Avançada para conteúdo no Microsoft Teams](/microsoft-365/compliance/teams-workflow-in-advanced-ediscovery) 


## <a name="permissions"></a>Permissões
Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).

|Tipo de permissão|Permissões (da com menos para a com mais privilégios)|
|:---|:---|
|Delegada (conta corporativa ou de estudante)|eDiscovery.ReadWrite.All|
|Delegada (conta pessoal da Microsoft)|Sem suporte.|
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
<!-- {
  "blockType": "request",
  "name": "ediscoverysearchthis.purgedata"
}
-->
``` http
POST https://graph.microsoft.com/beta/security/cases/eDiscoverycases/b0073e4e-4184-41c6-9eb7-8c8cc3e2288b/searches/c61a5860-d634-4d14-aea7-d82b6f4eb7af/purgeData
```


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