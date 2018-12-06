---
title: Obtenha os contatos do Outlook em uma pasta compartilhada
description: " Isso também é "
ms.openlocfilehash: c8c5b3a2eac49153826113af036146cc4475d9e5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27091588"
---
# <a name="get-outlook-contacts-in-a-shared-folder"></a><span data-ttu-id="49521-103">Obtenha os contatos do Outlook em uma pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="49521-103">Get Outlook contacts in a shared folder</span></span>

<span data-ttu-id="49521-104">Permite que os clientes do Outlook compartilhar pastas umas com as outras e forneça "ler", "criar", "modificar" ou "excluir" o acesso às pastas de contatos individuais.</span><span class="sxs-lookup"><span data-stu-id="49521-104">Outlook lets customers share folders with one another and provide "read", "create", "modify", or "delete" access to individual contact folders.</span></span> <span data-ttu-id="49521-105">O Outlook também permite que um cliente delegar a outro usuário para agir em nome do cliente e pastas específicas de acesso ou caixa de correio inteira do cliente; Isso também é conhecida como "delegação" no Outlook.</span><span class="sxs-lookup"><span data-stu-id="49521-105">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="49521-106">Programaticamente, o Microsoft Graph suporta obtendo contatos em pastas de contatos que foram compartilhadas por outros usuários, bem como introdução às próprias pastas compartilhadas.</span><span class="sxs-lookup"><span data-stu-id="49521-106">Programmatically, Microsoft Graph supports getting contacts in contact folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="49521-107">O suporte também se aplica às pastas em uma caixa de correio delegada.</span><span class="sxs-lookup"><span data-stu-id="49521-107">The support also applies to folders in a delegated mailbox.</span></span>

<span data-ttu-id="49521-108">Por exemplo, Garth tem compartilhadas com John uma pasta de contato personalizada e oferecido acesso de leitura de John.</span><span class="sxs-lookup"><span data-stu-id="49521-108">As an example, Garth has shared with John a custom contact folder and given John read access.</span></span> <span data-ttu-id="49521-109">Se John tiver entrado no seu aplicativo e oferecido permissões delegadas (Contacts.Read.Shared ou Contacts.ReadWrite.Shared), o seu aplicativo será capaz de acessar a pasta contato personalizada e os contatos nessa pasta, conforme descrito abaixo do Garth.</span><span class="sxs-lookup"><span data-stu-id="49521-109">If John has signed into your app and provided delegated permissions (Contacts.Read.Shared or Contacts.ReadWrite.Shared), your app will be able to access Garth's custom contact folder and contacts in that folder as described below.</span></span>

## <a name="get-a-contact-in-the-shared-folder"></a><span data-ttu-id="49521-110">Obtenha um contato na pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="49521-110">Get a contact in the shared folder</span></span>

<span data-ttu-id="49521-111">Você pode obter um contato específico na pasta contato personalizada que Garth tiver compartilhado com John:</span><span class="sxs-lookup"><span data-stu-id="49521-111">You can get a specific contact in the custom contact folder that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

<span data-ttu-id="49521-112">Após a conclusão bem-sucedida, você obterá HTTP 200 Okey e a instância de [contato](/graph/api/resources/contact?view=graph-rest-1.0) identificado pela `{id}` da pasta compartilhada de contato do Garth.</span><span class="sxs-lookup"><span data-stu-id="49521-112">On successful completion, you'll get HTTP 200 OK and the [contact](/graph/api/resources/contact?view=graph-rest-1.0) instance identified by `{id}` from Garth's shared contact folder.</span></span>

## <a name="get-all-contacts-in-the-shared-folder"></a><span data-ttu-id="49521-113">Obtenha todos os contatos na pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="49521-113">Get all contacts in the shared folder</span></span>

<span data-ttu-id="49521-114">Obtenha todos os contatos na pasta compartilhada de contato do Garth:</span><span class="sxs-lookup"><span data-stu-id="49521-114">Get all the contacts in Garth's shared contact folder:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

<span data-ttu-id="49521-115">Após a conclusão bem-sucedida, você obterá HTTP 200 Okey e um conjunto de instâncias de [contato](/graph/api/resources/contact?view=graph-rest-1.0) do Garth compartilhado a pasta de contato.</span><span class="sxs-lookup"><span data-stu-id="49521-115">On successful completion, you'll get HTTP 200 OK and a collection of [contact](/graph/api/resources/contact?view=graph-rest-1.0) instances in Garth's shared contact folder.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="49521-116">Obter a pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="49521-116">Get the shared folder</span></span>

<span data-ttu-id="49521-117">Obtenha a pasta de contato que Garth compartilhada com John.</span><span class="sxs-lookup"><span data-stu-id="49521-117">Get the contact folder that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

<span data-ttu-id="49521-118">Após a conclusão bem-sucedida, você obterá HTTP 200 Okey e compartilhados de uma instância de [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) que representa Garth pasta de contato.</span><span class="sxs-lookup"><span data-stu-id="49521-118">On successful completion, you'll get HTTP 200 OK and a [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) instance that represents Garth's shared contact folder.</span></span>

<span data-ttu-id="49521-119">Os mesmos recursos GET aplicam se Garth tinha delegada John sua caixa de correio inteira.</span><span class="sxs-lookup"><span data-stu-id="49521-119">The same GET capabilities apply if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="49521-120">Se Garth não compartilhou a pasta de contato com John, nem ele tem delegado sua caixa de correio de John, a especificação user ID do Garth ou o nome principal do usuário nessas operações GET retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="49521-120">If Garth has not shared the contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="49521-121">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="49521-121">Next steps</span></span>

<span data-ttu-id="49521-122">Saiba mais sobre:</span><span class="sxs-lookup"><span data-stu-id="49521-122">Find out more about:</span></span>

- [<span data-ttu-id="49521-123">Por que integram com contatos pessoais do Outlook</span><span class="sxs-lookup"><span data-stu-id="49521-123">Why integrate with Outlook personal contacts</span></span>](outlook-contacts-concept-overview.md)
- <span data-ttu-id="49521-124">Os [Contatos API](/graph/api/resources/contact?view=graph-rest-1.0) v 1.0 do Microsoft Graph.</span><span class="sxs-lookup"><span data-stu-id="49521-124">The [contacts API](/graph/api/resources/contact?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>