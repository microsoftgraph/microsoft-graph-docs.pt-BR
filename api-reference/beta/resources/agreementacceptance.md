---
title: tipo de recurso de agreementAcceptance
description: Representa o status atual de um usuário dentro do escopo dos termos de personalizável de uma empresa de uso possibilitada pela Azure Active Directory (AD Azure).
ms.openlocfilehash: 23221fe88a65b003c8d26aca99eaf1f03d935722
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27033143"
---
# <a name="agreementacceptance-resource-type"></a><span data-ttu-id="8f780-103">tipo de recurso de agreementAcceptance</span><span class="sxs-lookup"><span data-stu-id="8f780-103">agreementAcceptance resource type</span></span>

> <span data-ttu-id="8f780-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="8f780-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f780-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="8f780-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8f780-106">Representa o status atual de um usuário dentro do escopo dos termos de personalizável de uma empresa de uso possibilitada pela Azure Active Directory (AD Azure).</span><span class="sxs-lookup"><span data-stu-id="8f780-106">Represents the current status of a user within scope of a company's customizable terms of use powered by Azure Active Directory (Azure AD).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a><span data-ttu-id="8f780-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="8f780-107">Properties</span></span>
| <span data-ttu-id="8f780-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="8f780-108">Property</span></span>     | <span data-ttu-id="8f780-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="8f780-109">Type</span></span>        | <span data-ttu-id="8f780-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="8f780-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="8f780-111">agreementFileId</span><span class="sxs-lookup"><span data-stu-id="8f780-111">agreementFileId</span></span>|<span data-ttu-id="8f780-112">String</span><span class="sxs-lookup"><span data-stu-id="8f780-112">String</span></span>|<span data-ttu-id="8f780-113">ID do arquivo contrato aceito pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="8f780-113">ID of the agreement file accepted by the user.</span></span>|
|<span data-ttu-id="8f780-114">agreementId</span><span class="sxs-lookup"><span data-stu-id="8f780-114">agreementId</span></span>|<span data-ttu-id="8f780-115">String</span><span class="sxs-lookup"><span data-stu-id="8f780-115">String</span></span>|<span data-ttu-id="8f780-116">ID do contrato.</span><span class="sxs-lookup"><span data-stu-id="8f780-116">ID of the agreement.</span></span>|
|<span data-ttu-id="8f780-117">id</span><span class="sxs-lookup"><span data-stu-id="8f780-117">id</span></span>|<span data-ttu-id="8f780-118">String</span><span class="sxs-lookup"><span data-stu-id="8f780-118">String</span></span>| <span data-ttu-id="8f780-119">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="8f780-119">Read-only.</span></span>|
|<span data-ttu-id="8f780-120">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="8f780-120">recordedDateTime</span></span>|<span data-ttu-id="8f780-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8f780-121">DateTimeOffset</span></span>|<span data-ttu-id="8f780-p102">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="8f780-p102">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="8f780-124">state</span><span class="sxs-lookup"><span data-stu-id="8f780-124">state</span></span>|<span data-ttu-id="8f780-125">string</span><span class="sxs-lookup"><span data-stu-id="8f780-125">string</span></span>| <span data-ttu-id="8f780-126">Os valores possíveis são: `accepted` e `declined`.</span><span class="sxs-lookup"><span data-stu-id="8f780-126">Possible values are: `accepted`, `declined`.</span></span>|
|<span data-ttu-id="8f780-127">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="8f780-127">userDisplayName</span></span>|<span data-ttu-id="8f780-128">String</span><span class="sxs-lookup"><span data-stu-id="8f780-128">String</span></span>|<span data-ttu-id="8f780-129">Nome para exibição do usuário quando a aceitação foi registrada.</span><span class="sxs-lookup"><span data-stu-id="8f780-129">Display name of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="8f780-130">userEmail</span><span class="sxs-lookup"><span data-stu-id="8f780-130">userEmail</span></span>|<span data-ttu-id="8f780-131">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="8f780-131">String</span></span>|<span data-ttu-id="8f780-132">Email do usuário quando a aceitação foi registrada.</span><span class="sxs-lookup"><span data-stu-id="8f780-132">Email of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="8f780-133">userId</span><span class="sxs-lookup"><span data-stu-id="8f780-133">userId</span></span>|<span data-ttu-id="8f780-134">String</span><span class="sxs-lookup"><span data-stu-id="8f780-134">String</span></span>|<span data-ttu-id="8f780-135">ID do usuário que aceitou o contrato.</span><span class="sxs-lookup"><span data-stu-id="8f780-135">ID of the user who accepted the agreement.</span></span>|
|<span data-ttu-id="8f780-136">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8f780-136">userPrincipalName</span></span>|<span data-ttu-id="8f780-137">String</span><span class="sxs-lookup"><span data-stu-id="8f780-137">String</span></span>|<span data-ttu-id="8f780-138">UPN do usuário quando a aceitação foi registrada.</span><span class="sxs-lookup"><span data-stu-id="8f780-138">UPN of the user when the acceptance was recorded.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f780-139">Relações</span><span class="sxs-lookup"><span data-stu-id="8f780-139">Relationships</span></span>
<span data-ttu-id="8f780-140">Nenhum</span><span class="sxs-lookup"><span data-stu-id="8f780-140">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8f780-141">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="8f780-141">JSON representation</span></span>

<span data-ttu-id="8f780-142">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="8f780-142">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "agreementAcceptance resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
