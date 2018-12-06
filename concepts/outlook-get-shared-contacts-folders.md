---
title: Obter contatos do Outlook em uma pasta compartilhada
description: " isso também é "
ms.openlocfilehash: c8c5b3a2eac49153826113af036146cc4475d9e5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091588"
---
# <a name="get-outlook-contacts-in-a-shared-folder"></a><span data-ttu-id="1c2f4-103">Obter contatos do Outlook em uma pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="1c2f4-103">Get Outlook contacts in a shared folder</span></span>

<span data-ttu-id="1c2f4-104">O Outlook permite que os clientes compartilhem pastas entre si e forneçam acesso de "leitura", "criação", "modificação" ou "exclusão" a pastas de contatos individuais.</span><span class="sxs-lookup"><span data-stu-id="1c2f4-104">Outlook lets customers share folders with one another and provide "read", "create", or "modify" access to individual folders or the entire mailbox.</span></span> <span data-ttu-id="1c2f4-105">O Outlook também permite que um cliente delegue outro usuário para agir em nome do cliente e acesse pastas específicas ou toda a caixa de correio do cliente; isso também é conhecido como "delegação" no Outlook.</span><span class="sxs-lookup"><span data-stu-id="1c2f4-105">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="1c2f4-106">O Microsoft Graph oferece suporte de forma programática à obtenção de contatos em pastas de contatos que foram compartilhadas por outros usuários, além de receber as pastas compartilhadas em si.</span><span class="sxs-lookup"><span data-stu-id="1c2f4-106">Programmatically, Microsoft Graph supports getting messages in mail folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="1c2f4-107">O suporte também se aplica a pastas em uma caixa de correio delegada.</span><span class="sxs-lookup"><span data-stu-id="1c2f4-107">The support also applies to folders in a delegated mailbox.</span></span>

<span data-ttu-id="1c2f4-108">Por exemplo, Henrique compartilhou com Diogo uma pasta de contatos personalizada e deu a ele acesso de leitura.</span><span class="sxs-lookup"><span data-stu-id="1c2f4-108">As an example, Garth has shared with John a custom contact folder and given John read access.</span></span> <span data-ttu-id="1c2f4-109">Se Diogo se conectou ao seu aplicativo e forneceu permissões delegadas (Contacts.Read.Shared ou Contacts.ReadWrite.Shared), o aplicativo poderá acessar a pasta de contatos personalizada de Henrique e os contatos nessa pasta, conforme descrito abaixo.</span><span class="sxs-lookup"><span data-stu-id="1c2f4-109">If John has signed in your app and provided delegated permissions (Mail.Read.Shared or Mail.ReadWrite.Shared), your app will be able to access Garth's mail and Garth's Inbox as described below.</span></span>

## <a name="get-a-contact-in-the-shared-folder"></a><span data-ttu-id="1c2f4-110">Obter um contato na pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="1c2f4-110">Get a message in the shared folder</span></span>

<span data-ttu-id="1c2f4-111">Você pode obter um contato específico na pasta de contatos personalizada que Henrique compartilhou com Diogo:</span><span class="sxs-lookup"><span data-stu-id="1c2f4-111">You can get a specific contact in the custom contact folder that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

<span data-ttu-id="1c2f4-112">Após a conclusão bem-sucedida, você receberá HTTP 200 OK e a instância de [contact](/graph/api/resources/contact?view=graph-rest-1.0) identificada por `{id}` da pasta de contatos compartilhada de Henrique.</span><span class="sxs-lookup"><span data-stu-id="1c2f4-112">On successful completion, you'll get HTTP 200 OK and the [message](/graph/api/resources/contact?view=graph-rest-1.0) instance identified by `{id}` from Garth's Inbox.</span></span>

## <a name="get-all-contacts-in-the-shared-folder"></a><span data-ttu-id="1c2f4-113">Obter todos os contatos na pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="1c2f4-113">Get all messages in the shared folder</span></span>

<span data-ttu-id="1c2f4-114">Obtenha todos os contatos na pasta de contatos compartilhada do Henrique:</span><span class="sxs-lookup"><span data-stu-id="1c2f4-114">Get all the contacts in Garth's shared contact folder:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

<span data-ttu-id="1c2f4-115">Após a conclusão bem-sucedida, você receberá HTTP 200 OK e uma coleção de instâncias de [contact](/graph/api/resources/contact?view=graph-rest-1.0) na pasta de contatos compartilhada de Henrique.</span><span class="sxs-lookup"><span data-stu-id="1c2f4-115">On successful completion, you'll get HTTP 200 OK and a collection of [message](/graph/api/resources/contact?view=graph-rest-1.0) instances in Garth's Inbox.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="1c2f4-116">Obter a pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="1c2f4-116">Get the shared folder</span></span>

<span data-ttu-id="1c2f4-117">Obtenha a pasta de contatos que Henrique compartilhou com Diogo.</span><span class="sxs-lookup"><span data-stu-id="1c2f4-117">Get the folder (Inbox) that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

<span data-ttu-id="1c2f4-118">Após a conclusão bem-sucedida, você receberá HTTP 200 OK e uma instância de [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) que representa a pasta de contatos compartilhada de Henrique.</span><span class="sxs-lookup"><span data-stu-id="1c2f4-118">On successful completion, you'll get HTTP 200 OK and a [mailFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) instance that represents Garth's Inbox folder.</span></span>

<span data-ttu-id="1c2f4-119">As mesmas funcionalidades GET se aplicariam se Henrique tivesse delegado a Diogo toda a sua caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="1c2f4-119">The same GET capabilities apply if Garth had delegated John further access to Garth's Inbox, or if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="1c2f4-120">Se Henrique não tiver compartilhado sua pasta de contatos com Diogo nem delegado sua caixa de correio a Diogo, a especificação da ID de usuário de Henrique ou do nome UPN nessas operações GET retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="1c2f4-120">If Garth has not shared his contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="1c2f4-121">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="1c2f4-121">Next steps</span></span>

<span data-ttu-id="1c2f4-122">Saiba mais sobre:</span><span class="sxs-lookup"><span data-stu-id="1c2f4-122">Find out more about:</span></span>

- [<span data-ttu-id="1c2f4-123">Por que se integrar aos contatos pessoais do Outlook</span><span class="sxs-lookup"><span data-stu-id="1c2f4-123">Why integrate with Outlook personal contacts?</span></span>](outlook-contacts-concept-overview.md)
- <span data-ttu-id="1c2f4-124">A [API de contatos](/graph/api/resources/contact?view=graph-rest-1.0) do Outlook no Microsoft Graph v1.0.</span><span class="sxs-lookup"><span data-stu-id="1c2f4-124">The [contacts API](/graph/api/resources/contact?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>