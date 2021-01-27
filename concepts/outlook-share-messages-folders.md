---
title: Obter mensagens do Outlook em uma pasta compartilhada ou delegada
description: O Outlook permite que os clientes compartilhem pastas de e-mail entre si e forneçam acesso de "leitura", "criação", "modificação" ou "exclusão" a pastas individuais. O Outlook também permite que um cliente representante a outro usuário agir em nome do cliente.
author: angelgolfer-ms
localization_priority: Priority
ms.prod: outlook
ms.openlocfilehash: 6de4ee7ca1ed179bc538bb7aa1f2a3dacb8adb80
ms.sourcegitcommit: 6ec748ef00d025ee216274a608291be3c1257777
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/27/2021
ms.locfileid: "50013440"
---
# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a><span data-ttu-id="8097b-104">Obtenha mensagens do Outlook em uma pasta compartilhada ou delegada</span><span class="sxs-lookup"><span data-stu-id="8097b-104">Get Outlook messages in a shared or delegated folder</span></span>

<span data-ttu-id="8097b-105">O Outlook permite que os clientes compartilhem pastas de email entre si e forneçam acesso de "leitura", "criação", "modificação" ou "exclusão" a pastas individuais.</span><span class="sxs-lookup"><span data-stu-id="8097b-105">Outlook lets customers share mail folders with one another and provide "read", "create", "modify", or "delete" access to individual folders.</span></span> <span data-ttu-id="8097b-106">O Outlook também permite que um cliente delegue outro usuário para agir em nome do cliente e acesse pastas de correio específicas ou toda a caixa de correio do cliente; isso também é conhecido como "delegação" no Outlook.</span><span class="sxs-lookup"><span data-stu-id="8097b-106">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific mail folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="8097b-107">O Microsoft Graph oferece suporte de forma programática para receber mensagens em pastas de email que foram compartilhadas por outros usuários, além de receber as pastas compartilhadas em si.</span><span class="sxs-lookup"><span data-stu-id="8097b-107">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="8097b-108">O suporte também se aplica a pastas que foram delegadas.</span><span class="sxs-lookup"><span data-stu-id="8097b-108">The support also applies to folders that have been delegated.</span></span>

<span data-ttu-id="8097b-109">Por exemplo, Henrique compartilhou com Diogo e deu a ele acesso de leitura à sua caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="8097b-109">As an example, Garth has shared with John and given read access to Garth's Inbox.</span></span> <span data-ttu-id="8097b-110">Se Diogo estiver conectado em seu aplicativo e tiver fornecido permissões delegadas (Mail.Read.Shared ou Mail.ReadWrite.Shared), o aplicativo poderá acessar o email e a caixa de entrada do Henrique conforme descrito abaixo.</span><span class="sxs-lookup"><span data-stu-id="8097b-110">If John has signed into your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="microsoft-graph-permissions"></a><span data-ttu-id="8097b-111">Permissões do Microsoft Graph</span><span class="sxs-lookup"><span data-stu-id="8097b-111">Microsoft Graph permissions</span></span>

<span data-ttu-id="8097b-112">Use as permissões delegadas, `Mail.Read.Shared` ou `Mail.ReadWrite.Shared`, para ler ou gravar mensagens em uma pasta compartilhada ou delegada.</span><span class="sxs-lookup"><span data-stu-id="8097b-112">Use the delegated permissions, `Mail.Read.Shared` or `Mail.ReadWrite.Shared`, to respectively read or write messages in a shared or delegated folder.</span></span> 

<span data-ttu-id="8097b-113">Observe que essas duas permissões não são [para se inscrever para alterar as notificações](webhooks.md) em itens em pastas compartilhadas ou delegadas.</span><span class="sxs-lookup"><span data-stu-id="8097b-113">Note that those two permissions do not support [subscribing to change notifications](webhooks.md) on items in shared or delegated folders.</span></span> <span data-ttu-id="8097b-114">Para configurar assinaturas de notificação de alteração de mensagens em uma pasta de correio compartilhada, delegada, ou de qualquer outra pasta de correio de usuário no locatário, use a permissão do aplicativo,</span><span class="sxs-lookup"><span data-stu-id="8097b-114">To set up change notification subscriptions on messages in a shared, delegated, or any other user's mail folder in the tenant, use the application permission, `Mail.Read`.</span></span>

<span data-ttu-id="8097b-115">Saiba mais em [permissões de correio](permissions-reference.md#mail-permissions).</span><span class="sxs-lookup"><span data-stu-id="8097b-115">For more information, see [mail permissions](permissions-reference.md#mail-permissions).</span></span>

## <a name="get-a-message-in-the-shared-folder"></a><span data-ttu-id="8097b-116">Obtenha uma mensagem na pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="8097b-116">Get a message in the shared folder</span></span>

<span data-ttu-id="8097b-117">Você pode obter uma mensagem específica na caixa de entrada do Henrique:</span><span class="sxs-lookup"><span data-stu-id="8097b-117">You can get a specific message in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

<span data-ttu-id="8097b-118">Após a conclusão bem-sucedida, você receberá HTTP 200 OK e a instância de [message](/graph/api/resources/message) identificada por `{id}` da caixa de entrada do Henrique.</span><span class="sxs-lookup"><span data-stu-id="8097b-118">On successful completion, you'll get HTTP 200 OK and the [message](/graph/api/resources/message) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-messages-in-the-shared-folder"></a><span data-ttu-id="8097b-119">Obter todas as mensagens na pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="8097b-119">Get all messages in the shared folder</span></span>

<span data-ttu-id="8097b-120">Obtenha todas as mensagens na caixa de entrada do Henrique:</span><span class="sxs-lookup"><span data-stu-id="8097b-120">Get all the messages in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

<span data-ttu-id="8097b-121">Após a conclusão bem-sucedida, você receberá HTTP 200 OK um conjunto de instâncias de [message](/graph/api/resources/message) na caixa de entrada do Henrique.</span><span class="sxs-lookup"><span data-stu-id="8097b-121">On successful completion, you'll get HTTP 200 OK and a collection of [message](/graph/api/resources/message) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="8097b-122">Obter a pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="8097b-122">Get the shared folder</span></span>

<span data-ttu-id="8097b-123">Obtenha a pasta (caixa de entrada) que Henrique compartilhou com Diogo.</span><span class="sxs-lookup"><span data-stu-id="8097b-123">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

<span data-ttu-id="8097b-124">Após a conclusão bem-sucedida, você receberá HTTP 200 OK e uma instância de [mailFolder](/graph/api/resources/mailfolder) que representa a pasta de caixa de entrada do Henrique.</span><span class="sxs-lookup"><span data-stu-id="8097b-124">On successful completion, you'll get HTTP 200 OK and a [mailFolder](/graph/api/resources/mailfolder) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="8097b-125">Os mesmos recursos de GET se aplicam se Henrique delegar a Diogo mais acesso à sua caixa de entrada ou se Henrique delegar toda a sua caixa de correio a Diogo.</span><span class="sxs-lookup"><span data-stu-id="8097b-125">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="8097b-126">Se Henrique não tiver compartilhado sua caixa de entrada com Diogo nem delegado sua caixa de correio a Diogo, a especificação da ID de usuário de Henrique ou do nome de entidade de segurança nessas operações GET retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="8097b-126">If Garth has not shared his Inbox with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="8097b-127">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="8097b-127">Next steps</span></span>

<span data-ttu-id="8097b-128">Saiba mais sobre:</span><span class="sxs-lookup"><span data-stu-id="8097b-128">Find out more about:</span></span>

- [<span data-ttu-id="8097b-129">Por que integrar-se com o email do Outlook</span><span class="sxs-lookup"><span data-stu-id="8097b-129">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="8097b-130">[Como usar a API de email](/graph/api/resources/mail-api-overview) e seus [casos de uso](/graph/api/resources/mail-api-overview#common-use-cases) do Microsoft Graph versão 1.0.</span><span class="sxs-lookup"><span data-stu-id="8097b-130">[Using the mail API](/graph/api/resources/mail-api-overview) and its [use cases](/graph/api/resources/mail-api-overview#common-use-cases) in Microsoft Graph v1.0.</span></span>
