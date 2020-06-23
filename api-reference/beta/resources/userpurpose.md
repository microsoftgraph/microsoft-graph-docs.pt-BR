---
title: tipo de recurso userpurpose
description: Representa o tipo de destinatário ou de caixa de correio do usuário no Exchange Online.
localization_priority: Normal
doc_type: resourcePageType
ms.prod: outlook
author: abheek-das
ms.openlocfilehash: b4ed5db9dfa87b2829d78371339c166c3bb74265
ms.sourcegitcommit: b083a570375252eff8054f9fe70e1e5e2becc06d
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/23/2020
ms.locfileid: "44846370"
---
# <a name="userpurpose-resource-type"></a><span data-ttu-id="35875-103">tipo de recurso userpurpose</span><span class="sxs-lookup"><span data-stu-id="35875-103">userPurpose resource type</span></span>

<span data-ttu-id="35875-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="35875-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="35875-105">O objetivo da caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="35875-105">The purpose of the mailbox.</span></span> <span data-ttu-id="35875-106">Usado para diferenciar uma caixa de correio de um único usuário de uma caixa de correio compartilhada e caixa de correio de equipamento no Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="35875-106">Used to differentiate a mailbox for a single user from a shared mailbox and equipment mailbox in Exchange Online.</span></span>


## <a name="properties"></a><span data-ttu-id="35875-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="35875-107">Properties</span></span>
|<span data-ttu-id="35875-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35875-108">Property</span></span>|<span data-ttu-id="35875-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="35875-109">Type</span></span>|<span data-ttu-id="35875-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="35875-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="35875-111">valor</span><span class="sxs-lookup"><span data-stu-id="35875-111">value</span></span>|[<span data-ttu-id="35875-112">mailboxRecipientType</span><span class="sxs-lookup"><span data-stu-id="35875-112">mailboxRecipientType</span></span>](#mailboxrecipienttype-values)|<span data-ttu-id="35875-113">Representa o tipo de destinatário ou de caixa de correio do usuário no Exchange Online.</span><span class="sxs-lookup"><span data-stu-id="35875-113">Represents the user's recipient or mailbox type in Exchange Online.</span></span> <span data-ttu-id="35875-114">Os valores possíveis são: `unknown` , `user` , `linked` , `shared` , `room` , `equipment` e `others` .</span><span class="sxs-lookup"><span data-stu-id="35875-114">Possible values are: `unknown`, `user`, `linked`, `shared`, `room`, `equipment`, and `others`.</span></span> <span data-ttu-id="35875-115">Consulte a próxima seção para obter mais informações.</span><span class="sxs-lookup"><span data-stu-id="35875-115">See the next section for more information.</span></span>|

### <a name="mailboxrecipienttype-values"></a><span data-ttu-id="35875-116">valores de mailboxRecipientType</span><span class="sxs-lookup"><span data-stu-id="35875-116">mailboxRecipientType values</span></span>
|<span data-ttu-id="35875-117">Member</span><span class="sxs-lookup"><span data-stu-id="35875-117">Member</span></span>|<span data-ttu-id="35875-118">Descrição</span><span class="sxs-lookup"><span data-stu-id="35875-118">Description</span></span>|
|:---------------|:--------|
|<span data-ttu-id="35875-119">desconhecido</span><span class="sxs-lookup"><span data-stu-id="35875-119">unknown</span></span>|<span data-ttu-id="35875-120">Nenhuma informação encontrada sobre a caixa de correio.</span><span class="sxs-lookup"><span data-stu-id="35875-120">No information found about the mailbox.</span></span>|
|<span data-ttu-id="35875-121">usuário</span><span class="sxs-lookup"><span data-stu-id="35875-121">user</span></span>|<span data-ttu-id="35875-122">Uma conta de usuário com uma caixa de correio na floresta local.</span><span class="sxs-lookup"><span data-stu-id="35875-122">A user account with a mailbox in the local forest.</span></span>|
|<span data-ttu-id="35875-123">ligado</span><span class="sxs-lookup"><span data-stu-id="35875-123">linked</span></span>|<span data-ttu-id="35875-124">Uma caixa de correio vinculada a uma conta de usuário em outra floresta.</span><span class="sxs-lookup"><span data-stu-id="35875-124">A mailbox linked to a user account in another forest.</span></span>|
|<span data-ttu-id="35875-125">compartilhado</span><span class="sxs-lookup"><span data-stu-id="35875-125">shared</span></span>|<span data-ttu-id="35875-126">Uma caixa de correio compartilhada por duas ou mais contas de usuário.</span><span class="sxs-lookup"><span data-stu-id="35875-126">A mailbox shared by two or more user accounts.</span></span>|
|<span data-ttu-id="35875-127">cômodo</span><span class="sxs-lookup"><span data-stu-id="35875-127">room</span></span>|<span data-ttu-id="35875-128">Uma caixa de correio representando uma sala de conferência.</span><span class="sxs-lookup"><span data-stu-id="35875-128">A mailbox representing a conference room.</span></span>|
|<span data-ttu-id="35875-129">equipa</span><span class="sxs-lookup"><span data-stu-id="35875-129">equipment</span></span>|<span data-ttu-id="35875-130">Uma caixa de correio representando uma peça de equipamento.</span><span class="sxs-lookup"><span data-stu-id="35875-130">A mailbox representing a piece of equipment.</span></span>|
|<span data-ttu-id="35875-131">usuários</span><span class="sxs-lookup"><span data-stu-id="35875-131">others</span></span>|<span data-ttu-id="35875-132">Caixa de correio encontrada, mas o objetivo do usuário é diferente dos especificados acima.</span><span class="sxs-lookup"><span data-stu-id="35875-132">Mailbox found but user purpose is different from the ones specified above.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="35875-133">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="35875-133">JSON representation</span></span>

<span data-ttu-id="35875-134">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="35875-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userPurpose"
}-->

```json
{
    "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "userPurpose resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
