---
title: Obter contatos do Outlook em uma pasta compartilhada
description: O Outlook permite que os clientes compartilhem pastas entre si e forneçam acesso de "leitura", "criação", "modificação" ou "exclusão" a pastas de contatos individuais. O Outlook também permite que um cliente representante a outro usuário agir em nome do cliente.
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 86533a28c0af206458b63fd19f32f01c5b68710b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585437"
---
# <a name="get-outlook-contacts-in-a-shared-folder"></a><span data-ttu-id="7915e-104">Obter contatos do Outlook em uma pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="7915e-104">Get Outlook contacts in a shared folder</span></span>

<span data-ttu-id="7915e-105">O Outlook permite que os clientes compartilhem pastas entre si e forneçam acesso de "leitura", "criação", "modificação" ou "exclusão" a pastas de contatos individuais.</span><span class="sxs-lookup"><span data-stu-id="7915e-105">Outlook lets customers share folders with one another and provide "read", "create", "modify", or "delete" access to individual contact folders.</span></span> <span data-ttu-id="7915e-106">O Outlook também permite que um cliente delegue outro usuário para agir em nome do cliente e acesse pastas específicas ou toda a caixa de correio do cliente; isso também é conhecido como "delegação" no Outlook.</span><span class="sxs-lookup"><span data-stu-id="7915e-106">Outlook also allows a customer to delegate another user to act on the customer's behalf, and access specific folders or the customer's entire mailbox; this is also known as "delegation" in Outlook.</span></span>

<span data-ttu-id="7915e-107">O Microsoft Graph oferece suporte de forma programática à obtenção de contatos em pastas de contatos que foram compartilhadas por outros usuários, além de receber as pastas compartilhadas em si.</span><span class="sxs-lookup"><span data-stu-id="7915e-107">Programmatically, Microsoft Graph supports getting contacts in contact folders that have been shared by other users, as well as getting the shared folders themselves.</span></span> <span data-ttu-id="7915e-108">O suporte também se aplica a pastas em uma caixa de correio delegada.</span><span class="sxs-lookup"><span data-stu-id="7915e-108">The support also applies to folders in a delegated mailbox.</span></span>

<span data-ttu-id="7915e-109">Por exemplo, Henrique compartilhou com Diogo uma pasta de contatos personalizada e deu a ele acesso de leitura.</span><span class="sxs-lookup"><span data-stu-id="7915e-109">As an example, Garth has shared with John a custom contact folder and given John read access.</span></span> <span data-ttu-id="7915e-110">Se Diogo se conectou ao seu aplicativo e forneceu permissões delegadas (Contacts.Read.Shared ou Contacts.ReadWrite.Shared), o aplicativo poderá acessar a pasta de contatos personalizada de Henrique e os contatos nessa pasta, conforme descrito abaixo.</span><span class="sxs-lookup"><span data-stu-id="7915e-110">If John has signed into your app and provided delegated permissions (Contacts.Read.Shared or Contacts.ReadWrite.Shared), your app will be able to access Garth's custom contact folder and contacts in that folder as described below.</span></span>

> <span data-ttu-id="7915e-111">**Observação** permissões de compartilhamento (Contacts.Read.Shared ou Contacts.ReadWrite.Shared) permitem que a você ler ou escrever contatos em uma pasta compartilhada ou delegada.</span><span class="sxs-lookup"><span data-stu-id="7915e-111">**Note** The sharing permissions (Contacts.Read.Shared or Contacts.ReadWrite.Shared) allow you to read or write contacts in a shared or delegated folder.</span></span> <span data-ttu-id="7915e-112">Eles não têm suporte [subscrever alterar notificações](webhooks.md) em itens nessas pastas.</span><span class="sxs-lookup"><span data-stu-id="7915e-112">They do not support [subscribing to change notifications](webhooks.md) on items in such folders.</span></span> <span data-ttu-id="7915e-113">Para configurar as assinaturas de notificação de alteração nos contatos na pasta de contatos compartilhada, representante ou qualquer outra de um usuário no locatário, use a permissão de aplicativo Contacts.Read.</span><span class="sxs-lookup"><span data-stu-id="7915e-113">To set up change notification subscriptions on contacts in a shared, delegated, or any other user's contact folder in the tenant, use the application permission, Contacts.Read.</span></span>

## <a name="get-a-contact-in-the-shared-folder"></a><span data-ttu-id="7915e-114">Obter um contato na pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="7915e-114">Get a contact in the shared folder</span></span>

<span data-ttu-id="7915e-115">Você pode obter um contato específico na pasta de contatos personalizada que Henrique compartilhou com Diogo:</span><span class="sxs-lookup"><span data-stu-id="7915e-115">You can get a specific contact in the custom contact folder that Garth has shared with John:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts/{id}
```

<span data-ttu-id="7915e-116">Após a conclusão bem-sucedida, você receberá HTTP 200 OK e a instância de [contact](/graph/api/resources/contact?view=graph-rest-1.0) identificada por `{id}` da pasta de contatos compartilhada de Henrique.</span><span class="sxs-lookup"><span data-stu-id="7915e-116">On successful completion, you'll get HTTP 200 OK and the [contact](/graph/api/resources/contact?view=graph-rest-1.0) instance identified by `{id}` from Garth's shared contact folder.</span></span>

## <a name="get-all-contacts-in-the-shared-folder"></a><span data-ttu-id="7915e-117">Obter todos os contatos na pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="7915e-117">Get all contacts in the shared folder</span></span>

<span data-ttu-id="7915e-118">Obtenha todos os contatos na pasta de contatos compartilhada do Henrique:</span><span class="sxs-lookup"><span data-stu-id="7915e-118">Get all the contacts in Garth's shared contact folder:</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}/contacts
```

<span data-ttu-id="7915e-119">Após a conclusão bem-sucedida, você receberá HTTP 200 OK e uma coleção de instâncias de [contact](/graph/api/resources/contact?view=graph-rest-1.0) na pasta de contatos compartilhada de Henrique.</span><span class="sxs-lookup"><span data-stu-id="7915e-119">On successful completion, you'll get HTTP 200 OK and a collection of [contact](/graph/api/resources/contact?view=graph-rest-1.0) instances in Garth's shared contact folder.</span></span>

## <a name="get-the-shared-folder"></a><span data-ttu-id="7915e-120">Obter a pasta compartilhada</span><span class="sxs-lookup"><span data-stu-id="7915e-120">Get the shared folder</span></span>

<span data-ttu-id="7915e-121">Obtenha a pasta de contatos que Henrique compartilhou com Diogo.</span><span class="sxs-lookup"><span data-stu-id="7915e-121">Get the contact folder that Garth has shared with John.</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET users/{Garth-userId | Garth-userPrincipalName}/contactFolders/{folder-id}
```

<span data-ttu-id="7915e-122">Após a conclusão bem-sucedida, você receberá HTTP 200 OK e uma instância de [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) que representa a pasta de contatos compartilhada de Henrique.</span><span class="sxs-lookup"><span data-stu-id="7915e-122">On successful completion, you'll get HTTP 200 OK and a [contactFolder](/graph/api/resources/contactfolder?view=graph-rest-1.0) instance that represents Garth's shared contact folder.</span></span>

<span data-ttu-id="7915e-123">As mesmas funcionalidades GET se aplicariam se Henrique tivesse delegado a Diogo toda a sua caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="7915e-123">The same GET capabilities apply if Garth had delegated John his entire mailbox.</span></span>

<span data-ttu-id="7915e-124">Se Henrique não tiver compartilhado sua pasta de contatos com Diogo nem delegado sua caixa de correio a Diogo, a especificação da ID de usuário de Henrique ou do nome UPN nessas operações GET retornará um erro.</span><span class="sxs-lookup"><span data-stu-id="7915e-124">If Garth has not shared the contact folder with John, nor has he delegated his mailbox to John, specifying Garth’s user ID or user principal name in those GET operations will return an error.</span></span> 


## <a name="next-steps"></a><span data-ttu-id="7915e-125">Próximas etapas</span><span class="sxs-lookup"><span data-stu-id="7915e-125">Next steps</span></span>

<span data-ttu-id="7915e-126">Saiba mais sobre:</span><span class="sxs-lookup"><span data-stu-id="7915e-126">Find out more about:</span></span>

- [<span data-ttu-id="7915e-127">Por que se integrar aos contatos pessoais do Outlook</span><span class="sxs-lookup"><span data-stu-id="7915e-127">Why integrate with Outlook personal contacts</span></span>](outlook-contacts-concept-overview.md)
- <span data-ttu-id="7915e-128">A [API de contatos](/graph/api/resources/contact?view=graph-rest-1.0) do Outlook no Microsoft Graph v1.0.</span><span class="sxs-lookup"><span data-stu-id="7915e-128">The [contacts API](/graph/api/resources/contact?view=graph-rest-1.0) in Microsoft Graph v1.0.</span></span>
