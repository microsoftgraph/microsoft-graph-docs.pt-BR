---
title: tipo de recurso agreementAcceptance
description: Representa o status atual de um usuário dentro do escopo dos termos de uso personalizáveis de uma empresa, fornecido pelo Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 28f3c0adccb853ac8daddca9aaad70a2c0b35e2c
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508377"
---
# <a name="agreementacceptance-resource-type"></a><span data-ttu-id="f31b3-103">tipo de recurso agreementAcceptance</span><span class="sxs-lookup"><span data-stu-id="f31b3-103">agreementAcceptance resource type</span></span>

<span data-ttu-id="f31b3-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="f31b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f31b3-105">Representa o status atual de um usuário dentro do escopo dos termos de uso personalizáveis de uma empresa, fornecido pelo Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="f31b3-105">Represents the current status of a user within scope of a company's customizable terms of use powered by Azure Active Directory (Azure AD).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a><span data-ttu-id="f31b3-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="f31b3-106">Properties</span></span>
| <span data-ttu-id="f31b3-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="f31b3-107">Property</span></span>     | <span data-ttu-id="f31b3-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="f31b3-108">Type</span></span>        | <span data-ttu-id="f31b3-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="f31b3-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f31b3-110">agreementFileId</span><span class="sxs-lookup"><span data-stu-id="f31b3-110">agreementFileId</span></span>|<span data-ttu-id="f31b3-111">String</span><span class="sxs-lookup"><span data-stu-id="f31b3-111">String</span></span>|<span data-ttu-id="f31b3-112">ID do arquivo de contrato aceito pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="f31b3-112">ID of the agreement file accepted by the user.</span></span>|
|<span data-ttu-id="f31b3-113">agreementid</span><span class="sxs-lookup"><span data-stu-id="f31b3-113">agreementId</span></span>|<span data-ttu-id="f31b3-114">String</span><span class="sxs-lookup"><span data-stu-id="f31b3-114">String</span></span>|<span data-ttu-id="f31b3-115">ID do contrato.</span><span class="sxs-lookup"><span data-stu-id="f31b3-115">ID of the agreement.</span></span>|
|<span data-ttu-id="f31b3-116">id</span><span class="sxs-lookup"><span data-stu-id="f31b3-116">id</span></span>|<span data-ttu-id="f31b3-117">String</span><span class="sxs-lookup"><span data-stu-id="f31b3-117">String</span></span>| <span data-ttu-id="f31b3-118">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="f31b3-118">Read-only.</span></span>|
|<span data-ttu-id="f31b3-119">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="f31b3-119">recordedDateTime</span></span>|<span data-ttu-id="f31b3-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f31b3-120">DateTimeOffset</span></span>|<span data-ttu-id="f31b3-p101">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f31b3-p101">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f31b3-123">estado</span><span class="sxs-lookup"><span data-stu-id="f31b3-123">state</span></span>|<span data-ttu-id="f31b3-124">string</span><span class="sxs-lookup"><span data-stu-id="f31b3-124">string</span></span>| <span data-ttu-id="f31b3-125">Os valores possíveis são: `accepted` e `declined`.</span><span class="sxs-lookup"><span data-stu-id="f31b3-125">Possible values are: `accepted`, `declined`.</span></span>|
|<span data-ttu-id="f31b3-126">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="f31b3-126">userDisplayName</span></span>|<span data-ttu-id="f31b3-127">String</span><span class="sxs-lookup"><span data-stu-id="f31b3-127">String</span></span>|<span data-ttu-id="f31b3-128">Nome para exibição do usuário quando a aceitação foi registrada.</span><span class="sxs-lookup"><span data-stu-id="f31b3-128">Display name of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="f31b3-129">userEmail</span><span class="sxs-lookup"><span data-stu-id="f31b3-129">userEmail</span></span>|<span data-ttu-id="f31b3-130">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="f31b3-130">String</span></span>|<span data-ttu-id="f31b3-131">Email do usuário quando a aceitação foi registrada.</span><span class="sxs-lookup"><span data-stu-id="f31b3-131">Email of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="f31b3-132">userId</span><span class="sxs-lookup"><span data-stu-id="f31b3-132">userId</span></span>|<span data-ttu-id="f31b3-133">String</span><span class="sxs-lookup"><span data-stu-id="f31b3-133">String</span></span>|<span data-ttu-id="f31b3-134">ID do usuário que aceitou o contrato.</span><span class="sxs-lookup"><span data-stu-id="f31b3-134">ID of the user who accepted the agreement.</span></span>|
|<span data-ttu-id="f31b3-135">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f31b3-135">userPrincipalName</span></span>|<span data-ttu-id="f31b3-136">String</span><span class="sxs-lookup"><span data-stu-id="f31b3-136">String</span></span>|<span data-ttu-id="f31b3-137">UPN do usuário quando a aceitação foi registrada.</span><span class="sxs-lookup"><span data-stu-id="f31b3-137">UPN of the user when the acceptance was recorded.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f31b3-138">Relações</span><span class="sxs-lookup"><span data-stu-id="f31b3-138">Relationships</span></span>
<span data-ttu-id="f31b3-139">Nenhum</span><span class="sxs-lookup"><span data-stu-id="f31b3-139">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f31b3-140">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="f31b3-140">JSON representation</span></span>

<span data-ttu-id="f31b3-141">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="f31b3-141">The following is a JSON representation of the resource.</span></span>

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
