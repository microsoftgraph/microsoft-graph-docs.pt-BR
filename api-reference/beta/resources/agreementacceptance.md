---
title: tipo de recurso agreementAcceptance
description: Representa o status atual de um usuário dentro do escopo dos termos de uso personalizáveis de uma empresa, fornecido pelo Azure Active Directory (Azure AD).
localization_priority: Normal
ms.openlocfilehash: 84b54998e8afaad501d2cf46d564400aa2307507
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339138"
---
# <a name="agreementacceptance-resource-type"></a><span data-ttu-id="b54cd-103">tipo de recurso agreementAcceptance</span><span class="sxs-lookup"><span data-stu-id="b54cd-103">agreementAcceptance resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b54cd-104">Representa o status atual de um usuário dentro do escopo dos termos de uso personalizáveis de uma empresa, fornecido pelo Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="b54cd-104">Represents the current status of a user within scope of a company's customizable terms of use powered by Azure Active Directory (Azure AD).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a><span data-ttu-id="b54cd-105">Propriedades</span><span class="sxs-lookup"><span data-stu-id="b54cd-105">Properties</span></span>
| <span data-ttu-id="b54cd-106">Propriedade</span><span class="sxs-lookup"><span data-stu-id="b54cd-106">Property</span></span>     | <span data-ttu-id="b54cd-107">Tipo</span><span class="sxs-lookup"><span data-stu-id="b54cd-107">Type</span></span>        | <span data-ttu-id="b54cd-108">Descrição</span><span class="sxs-lookup"><span data-stu-id="b54cd-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b54cd-109">agreementFileId</span><span class="sxs-lookup"><span data-stu-id="b54cd-109">agreementFileId</span></span>|<span data-ttu-id="b54cd-110">String</span><span class="sxs-lookup"><span data-stu-id="b54cd-110">String</span></span>|<span data-ttu-id="b54cd-111">ID do arquivo de contrato aceito pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="b54cd-111">ID of the agreement file accepted by the user.</span></span>|
|<span data-ttu-id="b54cd-112">agreementid</span><span class="sxs-lookup"><span data-stu-id="b54cd-112">agreementId</span></span>|<span data-ttu-id="b54cd-113">String</span><span class="sxs-lookup"><span data-stu-id="b54cd-113">String</span></span>|<span data-ttu-id="b54cd-114">ID do contrato.</span><span class="sxs-lookup"><span data-stu-id="b54cd-114">ID of the agreement.</span></span>|
|<span data-ttu-id="b54cd-115">id</span><span class="sxs-lookup"><span data-stu-id="b54cd-115">id</span></span>|<span data-ttu-id="b54cd-116">String</span><span class="sxs-lookup"><span data-stu-id="b54cd-116">String</span></span>| <span data-ttu-id="b54cd-117">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="b54cd-117">Read-only.</span></span>|
|<span data-ttu-id="b54cd-118">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="b54cd-118">recordedDateTime</span></span>|<span data-ttu-id="b54cd-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b54cd-119">DateTimeOffset</span></span>|<span data-ttu-id="b54cd-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b54cd-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b54cd-122">estado</span><span class="sxs-lookup"><span data-stu-id="b54cd-122">state</span></span>|<span data-ttu-id="b54cd-123">string</span><span class="sxs-lookup"><span data-stu-id="b54cd-123">string</span></span>| <span data-ttu-id="b54cd-124">Os valores possíveis são: `accepted` e `declined`.</span><span class="sxs-lookup"><span data-stu-id="b54cd-124">Possible values are: `accepted`, `declined`.</span></span>|
|<span data-ttu-id="b54cd-125">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="b54cd-125">userDisplayName</span></span>|<span data-ttu-id="b54cd-126">String</span><span class="sxs-lookup"><span data-stu-id="b54cd-126">String</span></span>|<span data-ttu-id="b54cd-127">Nome para exibição do usuário quando a aceitação foi registrada.</span><span class="sxs-lookup"><span data-stu-id="b54cd-127">Display name of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="b54cd-128">userEmail</span><span class="sxs-lookup"><span data-stu-id="b54cd-128">userEmail</span></span>|<span data-ttu-id="b54cd-129">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="b54cd-129">String</span></span>|<span data-ttu-id="b54cd-130">Email do usuário quando a aceitação foi registrada.</span><span class="sxs-lookup"><span data-stu-id="b54cd-130">Email of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="b54cd-131">userId</span><span class="sxs-lookup"><span data-stu-id="b54cd-131">userId</span></span>|<span data-ttu-id="b54cd-132">String</span><span class="sxs-lookup"><span data-stu-id="b54cd-132">String</span></span>|<span data-ttu-id="b54cd-133">ID do usuário que aceitou o contrato.</span><span class="sxs-lookup"><span data-stu-id="b54cd-133">ID of the user who accepted the agreement.</span></span>|
|<span data-ttu-id="b54cd-134">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b54cd-134">userPrincipalName</span></span>|<span data-ttu-id="b54cd-135">String</span><span class="sxs-lookup"><span data-stu-id="b54cd-135">String</span></span>|<span data-ttu-id="b54cd-136">UPN do usuário quando a aceitação foi registrada.</span><span class="sxs-lookup"><span data-stu-id="b54cd-136">UPN of the user when the acceptance was recorded.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b54cd-137">Relações</span><span class="sxs-lookup"><span data-stu-id="b54cd-137">Relationships</span></span>
<span data-ttu-id="b54cd-138">Nenhum</span><span class="sxs-lookup"><span data-stu-id="b54cd-138">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b54cd-139">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="b54cd-139">JSON representation</span></span>

<span data-ttu-id="b54cd-140">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="b54cd-140">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementAcceptance"
}-->

```json
{
  "agreementFileId": "String",
  "agreementId": "String",
  "id": "String (identifier)",
  "recordedDateTime": "String (timestamp)",
  "state": "string",
  "userDisplayName": "String",
  "userEmail": "String",
  "userId": "String",
  "userPrincipalName": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementAcceptance resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
