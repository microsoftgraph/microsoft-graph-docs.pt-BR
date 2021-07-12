---
author: nkramer
ms.topic: include
ms.date: 01/25/2021
ms.openlocfilehash: f3854b06c7d4dc584a922f9c454947785b74947f
ms.sourcegitcommit: 3873c85f53e026073addca92d31d234af244444c
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/12/2021
ms.locfileid: "53005746"
---
<!-- markdownlint-disable MD041-->

### <a name="chatmessage"></a><span data-ttu-id="468d7-101">chatMessage</span><span class="sxs-lookup"><span data-stu-id="468d7-101">chatMessage</span></span>

<span data-ttu-id="468d7-102">**chatMessage** assinaturas com permissões delegadas não oferecem suporte a dados de recursos (**includeResourceData** deve ser `false`) e não requerem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="468d7-102">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="468d7-103">Assinaturas **chatMessage** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="468d7-103">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="468d7-104">A criação da assinatura falhará se [encryptionCertificate](/graph/api/resources/subscription) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="468d7-104">Subscription creation will fail if [encryptionCertificate](/graph/api/resources/subscription) is not specified.</span></span> <span data-ttu-id="468d7-105">Antes de criar uma assinatura **chatMessage**, você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="468d7-105">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="468d7-106">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="468d7-106">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="468d7-107">**Observações:**</span><span class="sxs-lookup"><span data-stu-id="468d7-107">**Notes:**</span></span> 
>
><span data-ttu-id="468d7-p102">`/teams/getAllMessages` e `/chats/getAllMessages` estão disponíveis para os usuários que possuem as [licenças necessárias](https://aka.ms/teams-changenotification-licenses). No futuro, a Microsoft poderá exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados acessados através da API.</span><span class="sxs-lookup"><span data-stu-id="468d7-p102">`/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses). In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>
