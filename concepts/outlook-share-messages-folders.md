---
title: Obter mensagens do Outlook em uma pasta compartilhada ou delegada
description: 'Esses tópicos também têm eventos similares de lista de seções: obter evento, obter calendário, listar contatos, obter contato, obter a pasta de contatos.'
author: angelgolfer-ms
ms.openlocfilehash: d90fa5d37fd7a07e4069bd5bcc0eb46f0cae29a6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27320108"
---
# <a name="get-outlook-messages-in-a-shared-or-delegated-folder"></a><span data-ttu-id="000ba-103">Obter mensagens do Outlook em uma pasta compartilhada ou delegada</span><span class="sxs-lookup"><span data-stu-id="000ba-103">Get Outlook messages in a shared or delegated folder</span></span>

<!-- remove similar content in other topics when ready to publish - list messages, get message, get mail folder.
These topics also have similar section - list events, get event, get calendar, list contacts, get contact, get contact folder.
-->

<span data-ttu-id="000ba-104">O Outlook permite que os clientes compartilhem pastas de email entre si e forneçam acesso de "leitura", "criação", "modificação" ou "exclusão" a pastas individuais.</span><span class="sxs-lookup"><span data-stu-id="000ba-104">Outlook lets customers share mail folders with one another and provide "read", "create", "modify", or "delete" access to individual folders.</span></span> <span data-ttu-id="000ba-105">O Outlook também permite que um cliente delegue outro usuário para agir em nome do cliente e acesse pastas de correio específicas ou toda a caixa de correio do cliente; isso também é conhecido como "delegação" no Outlook.</span><span class="sxs-lookup"><span data-stu-id="000ba-105">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific mail folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="000ba-106">O Microsoft Graph oferece suporte de forma programática para receber mensagens em pastas de email que foram compartilhadas por outros usuários, além de receber as pastas compartilhadas em si.</span><span class="sxs-lookup"><span data-stu-id="000ba-106">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="000ba-107">O suporte também se aplica a pastas que foram delegadas.</span><span class="sxs-lookup"><span data-stu-id="000ba-107">The support also applies to folders that have been delegated.</span></span>

<span data-ttu-id="000ba-108">Por exemplo, Henrique compartilhou com Diogo e deu a ele acesso de leitura à sua caixa de entrada.</span><span class="sxs-lookup"><span data-stu-id="000ba-108">As an example, Garth has shared with John and given read access to Garth's Inbox.</span></span> <span data-ttu-id="000ba-109">Se Diogo estiver conectado em seu aplicativo e tiver fornecido permissões delegadas (Mail.Read.Shared ou Mail.ReadWrite.Shared), o aplicativo poderá acessar o email e a caixa de entrada do Henrique conforme descrito abaixo.</span><span class="sxs-lookup"><span data-stu-id="000ba-109">If John has signed into your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-a-message-in-the-shared-folder"></a><span data-ttu-id="000ba-110">Obter uma mensagem na pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="000ba-110">Get a message in the shared folder</span></span>

<span data-ttu-id="000ba-111">Você pode obter uma mensagem específica na caixa de entrada do Henrique:</span><span class="sxs-lookup"><span data-stu-id="000ba-111">You can get a specific message in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages/{id}
```

<span data-ttu-id="000ba-112">Após a conclusão bem-sucedida, você receberá HTTP 200 OK e a instância de [message](/graph/api/resources/message?view=graph-rest-1.0) identificada por `{id}` da caixa de entrada do Henrique.</span><span class="sxs-lookup"><span data-stu-id="000ba-112">On successful completion, you'll get HTTP 200 OK and the [message](/graph/api/resources/message?view=graph-rest-1.0) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-messages-in-the-shared-folder"></a><span data-ttu-id="000ba-113">Obter todas as mensagens na pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="000ba-113">Get all messages in the shared folder</span></span>

<span data-ttu-id="000ba-114">Obtenha todas as mensagens na caixa de entrada do Henrique:</span><span class="sxs-lookup"><span data-stu-id="000ba-114">Get all the messages in Garth's Inbox:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')/messages
```

<span data-ttu-id="000ba-115">Após a conclusão bem-sucedida, você receberá HTTP 200 OK um conjunto de instâncias de [message](/graph/api/resources/message?view=graph-rest-1.0) na caixa de entrada do Henrique.</span><span class="sxs-lookup"><span data-stu-id="000ba-115">On successful completion, you'll get HTTP 200 OK and a collection of [message](/graph/api/resources/message?view=graph-rest-1.0) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="000ba-116">Obter a pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="000ba-116">Get the shared folder</span></span>

<span data-ttu-id="000ba-117">Obtenha a pasta (caixa de entrada) que Henrique compartilhou com Diogo.</span><span class="sxs-lookup"><span data-stu-id="000ba-117">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/mailfolders('Inbox')
```

<span data-ttu-id="000ba-118">Após a conclusão bem-sucedida, você receberá HTTP 200 OK e uma instância de [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) que representa a pasta de caixa de entrada do Henrique.</span><span class="sxs-lookup"><span data-stu-id="000ba-118">On successful completion, you'll get HTTP 200 OK and a [mailFolder](/graph/api/resources/mailfolder?view=graph-rest-1.0) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="000ba-119">Os mesmos recursos de GET se aplicam se Henrique delegar a Diogo mais acesso à sua caixa de entrada ou se Henrique delegar toda a sua caixa de correio a Diogo.</span><span class="sxs-lookup"><span data-stu-id="000ba-119">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="000ba-120">Se Henrique não tiver compartilhado sua caixa de entrada com Diogo nem delegado sua caixa de correio a Diogo, a especificação da ID de usuário de Henrique ou do nome de entidade de segurança nessas operações GET retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="000ba-120">If Garth has not shared his Inbox with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="000ba-121">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="000ba-121">Next steps</span></span>

<span data-ttu-id="000ba-122">Saiba mais sobre:</span><span class="sxs-lookup"><span data-stu-id="000ba-122">Find out more about:</span></span>

- [<span data-ttu-id="000ba-123">Por que integrar-se com o email do Outlook</span><span class="sxs-lookup"><span data-stu-id="000ba-123">Why integrate with Outlook mail</span></span>](outlook-mail-concept-overview.md)
- <span data-ttu-id="000ba-124">[Como usar a API de email](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) e seus [casos de uso](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) do Microsoft Graph versão 1.0.</span><span class="sxs-lookup"><span data-stu-id="000ba-124">[Using the mail API](/graph/api/resources/mail-api-overview?view=graph-rest-1.0) and its [use cases](/graph/api/resources/mail-api-overview?view=graph-rest-1.0#common-use-cases) in Microsoft Graph v1.0.</span></span>