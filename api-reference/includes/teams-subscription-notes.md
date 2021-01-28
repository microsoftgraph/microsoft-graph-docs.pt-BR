---
author: nkramer
ms.topic: include
ms.date: 01/25/2021
ms.author: nkramer
ms.openlocfilehash: ef6cf05f93a8a7f33926ba253e9241bb4c445ad1
ms.sourcegitcommit: 9a03b719d1316729dd022bf4d268894e91515475
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/28/2021
ms.locfileid: "50034070"
---
<!-- markdownlint-disable MD041-->

### <a name="chatmessage"></a><span data-ttu-id="c9258-101">chatMessage</span><span class="sxs-lookup"><span data-stu-id="c9258-101">chatMessage</span></span>

<span data-ttu-id="c9258-102">**chatMessage** assinaturas com permissões delegadas não oferecem suporte a dados de recursos (**includeResourceData** deve ser `false`) e não requerem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="c9258-102">**chatMessage** subscriptions with delegated permissions do not support resource data (**includeResourceData** must be `false`), and do not require [encryption](/graph/webhooks-with-resource-data).</span></span>

<span data-ttu-id="c9258-103">Assinaturas **chatMessage** com permissões de aplicativo incluem dados de recurso e exigem [criptografia](/graph/webhooks-with-resource-data).</span><span class="sxs-lookup"><span data-stu-id="c9258-103">**chatMessage** subscriptions with application permissions include resource data, and require [encryption](/graph/webhooks-with-resource-data).</span></span> <span data-ttu-id="c9258-104">A criação da assinatura falhará se [encryptionCertificate](/graph/api/resources/subscription) não for especificado.</span><span class="sxs-lookup"><span data-stu-id="c9258-104">Subscription creation will fail if [encryptionCertificate](/graph/api/resources/subscription) is not specified.</span></span> <span data-ttu-id="c9258-105">Antes de criar uma assinatura **chatMessage**, você deve solicitar acesso.</span><span class="sxs-lookup"><span data-stu-id="c9258-105">Before creating a **chatMessage** subscription, you must request access.</span></span> <span data-ttu-id="c9258-106">Para obter detalhes, confira [APIs protegidas no Microsoft Teams](/graph/teams-protected-apis).</span><span class="sxs-lookup"><span data-stu-id="c9258-106">For details, see [Protected APIs in Microsoft Teams](/graph/teams-protected-apis).</span></span> 

> <span data-ttu-id="c9258-107">**Observações:**</span><span class="sxs-lookup"><span data-stu-id="c9258-107">**Notes:**</span></span> 
>
><span data-ttu-id="c9258-108">`/teams/getAllMessages` e `/chats/getAllMessages` estão disponíveis para usuários que possuem as [licenças necessárias](https://aka.ms/teams-changenotification-licenses).</span><span class="sxs-lookup"><span data-stu-id="c9258-108">`/teams/getAllMessages` and `/chats/getAllMessages` are available to users that have the [required licenses](https://aka.ms/teams-changenotification-licenses).</span></span>
<span data-ttu-id="c9258-109">No futuro, a Microsoft poderá exigir que você ou seus clientes paguem taxas adicionais com base na quantidade de dados acessados pela API.</span><span class="sxs-lookup"><span data-stu-id="c9258-109">In the future, Microsoft may require you or your customers to pay additional fees based on the amount of data accessed through the API.</span></span>
>
><span data-ttu-id="c9258-110">`/chats/getAllMessages` retorna apenas mensagens de bate-papos pertencentes ao locatário.</span><span class="sxs-lookup"><span data-stu-id="c9258-110">`/chats/getAllMessages` only returns messages from chats owned by the tenant.</span></span> <span data-ttu-id="c9258-111">Se um thread de bate papo for iniciado por um usuário fora do locatário, esse thread de bate papo não será de propriedade do locatário e não criará notificações de alteração.</span><span class="sxs-lookup"><span data-stu-id="c9258-111">If a chat thread is initiated by a user outside the tenant, that chat thread is not owned by the tenant, and does not create change notifications.</span></span>
