---
title: Tipo de recurso agreementAcceptance
description: Representa o status atual de um usuário dentro do escopo dos termos de uso personalizáveis de uma empresa com o Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: raprakasMSFT
ms.openlocfilehash: 55e0be212c0f7a9e655acff03606eda851a0e5c6
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722479"
---
# <a name="agreementacceptance-resource-type"></a><span data-ttu-id="e6590-103">Tipo de recurso agreementAcceptance</span><span class="sxs-lookup"><span data-stu-id="e6590-103">agreementAcceptance resource type</span></span>

<span data-ttu-id="e6590-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6590-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e6590-105">Representa o status atual de um usuário dentro do escopo dos termos de uso personalizáveis de uma empresa com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="e6590-105">Represents the current status of a user within scope of a company's customizable terms of use powered by Azure Active Directory (Azure AD).</span></span>

<!--
## Methods

| Method       | Return Type | Description |
|:-------------|:------------|:------------|
| [Get agreementAcceptance](../api/agreementacceptance-get.md) | [agreementAcceptance](agreementacceptance.md) | Read properties and relationships of agreementAcceptance object. |
| [Update](../api/agreementacceptance-update.md) | [agreementAcceptance](agreementacceptance.md) | Update an **agreementAcceptance** object. |
| [Delete](../api/agreementacceptance-delete.md) | None | Delete an **agreementAcceptance** object. |
-->

## <a name="properties"></a><span data-ttu-id="e6590-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6590-106">Properties</span></span>
| <span data-ttu-id="e6590-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6590-107">Property</span></span>     | <span data-ttu-id="e6590-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6590-108">Type</span></span>        | <span data-ttu-id="e6590-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6590-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e6590-110">agreementFileId</span><span class="sxs-lookup"><span data-stu-id="e6590-110">agreementFileId</span></span>|<span data-ttu-id="e6590-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6590-111">String</span></span>|<span data-ttu-id="e6590-112">ID do arquivo de contrato aceito pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="e6590-112">ID of the agreement file accepted by the user.</span></span>|
|<span data-ttu-id="e6590-113">agreementId</span><span class="sxs-lookup"><span data-stu-id="e6590-113">agreementId</span></span>|<span data-ttu-id="e6590-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6590-114">String</span></span>|<span data-ttu-id="e6590-115">ID do contrato.</span><span class="sxs-lookup"><span data-stu-id="e6590-115">ID of the agreement.</span></span>|
|<span data-ttu-id="e6590-116">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="e6590-116">deviceDisplayName</span></span>|<span data-ttu-id="e6590-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6590-117">String</span></span>|<span data-ttu-id="e6590-118">O nome de exibição do dispositivo usado para aceitar o contrato.</span><span class="sxs-lookup"><span data-stu-id="e6590-118">The display name of the device used for accepting the agreement.</span></span>|
|<span data-ttu-id="e6590-119">deviceId</span><span class="sxs-lookup"><span data-stu-id="e6590-119">deviceId</span></span>|<span data-ttu-id="e6590-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6590-120">String</span></span>|<span data-ttu-id="e6590-121">O identificador exclusivo do dispositivo usado para aceitar o contrato.</span><span class="sxs-lookup"><span data-stu-id="e6590-121">The unique identifier of the device used for accepting the agreement.</span></span>|
|<span data-ttu-id="e6590-122">deviceOSType</span><span class="sxs-lookup"><span data-stu-id="e6590-122">deviceOSType</span></span>|<span data-ttu-id="e6590-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6590-123">String</span></span>|<span data-ttu-id="e6590-124">O sistema operacional usado para aceitar o contrato.</span><span class="sxs-lookup"><span data-stu-id="e6590-124">The operating system used for accepting the agreement.</span></span>|
|<span data-ttu-id="e6590-125">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="e6590-125">deviceOSVersion</span></span>|<span data-ttu-id="e6590-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6590-126">String</span></span>|<span data-ttu-id="e6590-127">A versão do sistema operacional do dispositivo usado para aceitar o contrato.</span><span class="sxs-lookup"><span data-stu-id="e6590-127">The operating system version of the device used for accepting the agreement.</span></span>    |
|<span data-ttu-id="e6590-128">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e6590-128">expirationDateTime</span></span>|<span data-ttu-id="e6590-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6590-129">DateTimeOffset</span></span>|<span data-ttu-id="e6590-130">A data de expiração da aceitação.</span><span class="sxs-lookup"><span data-stu-id="e6590-130">The expiration date time of the acceptance.</span></span> <span data-ttu-id="e6590-131">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="e6590-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e6590-132">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="e6590-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="e6590-133">id</span><span class="sxs-lookup"><span data-stu-id="e6590-133">id</span></span>|<span data-ttu-id="e6590-134">String</span><span class="sxs-lookup"><span data-stu-id="e6590-134">String</span></span>| <span data-ttu-id="e6590-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6590-135">Read-only.</span></span>|
|<span data-ttu-id="e6590-136">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6590-136">recordedDateTime</span></span>|<span data-ttu-id="e6590-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6590-137">DateTimeOffset</span></span>|<span data-ttu-id="e6590-138">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="e6590-138">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e6590-139">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="e6590-139">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="e6590-140">estado</span><span class="sxs-lookup"><span data-stu-id="e6590-140">state</span></span>|<span data-ttu-id="e6590-141">string</span><span class="sxs-lookup"><span data-stu-id="e6590-141">string</span></span>| <span data-ttu-id="e6590-142">Os valores possíveis são: `accepted` e `declined`.</span><span class="sxs-lookup"><span data-stu-id="e6590-142">Possible values are: `accepted`, `declined`.</span></span>|
|<span data-ttu-id="e6590-143">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e6590-143">userDisplayName</span></span>|<span data-ttu-id="e6590-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6590-144">String</span></span>|<span data-ttu-id="e6590-145">Nome de exibição do usuário quando a aceitação foi registrada.</span><span class="sxs-lookup"><span data-stu-id="e6590-145">Display name of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="e6590-146">userEmail</span><span class="sxs-lookup"><span data-stu-id="e6590-146">userEmail</span></span>|<span data-ttu-id="e6590-147">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6590-147">String</span></span>|<span data-ttu-id="e6590-148">Email do usuário quando a aceitação foi registrada.</span><span class="sxs-lookup"><span data-stu-id="e6590-148">Email of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="e6590-149">userId</span><span class="sxs-lookup"><span data-stu-id="e6590-149">userId</span></span>|<span data-ttu-id="e6590-150">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6590-150">String</span></span>|<span data-ttu-id="e6590-151">ID do usuário que aceitou o contrato.</span><span class="sxs-lookup"><span data-stu-id="e6590-151">ID of the user who accepted the agreement.</span></span>|
|<span data-ttu-id="e6590-152">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e6590-152">userPrincipalName</span></span>|<span data-ttu-id="e6590-153">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6590-153">String</span></span>|<span data-ttu-id="e6590-154">UPN do usuário quando a aceitação foi registrada.</span><span class="sxs-lookup"><span data-stu-id="e6590-154">UPN of the user when the acceptance was recorded.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6590-155">Relações</span><span class="sxs-lookup"><span data-stu-id="e6590-155">Relationships</span></span>
<span data-ttu-id="e6590-156">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6590-156">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e6590-157">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6590-157">JSON representation</span></span>

<span data-ttu-id="e6590-158">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e6590-158">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementAcceptance"
}-->

```json
{
      "id": "String (identifier)",
      "agreementId": "String",
      "userId": "String",
      "deviceId": "String",
      "deviceDisplayName": "String",
      "deviceOSType": "String",
      "deviceOSVersion": "String",
      "agreementFileId": "String",
      "userDisplayName": "String",
      "userPrincipalName": "String",
      "userEmail": "String",
      "recordedDateTime": "String (timestamp)",
      "expirationDateTime": "String",
      "state": "String"
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


