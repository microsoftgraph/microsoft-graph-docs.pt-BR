---
title: Tipo de recurso agreementAcceptance
description: Representa o status atual de um usuário dentro do escopo dos termos de uso personalizáveis de uma empresa com o Azure Active Directory (Azure AD).
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: raprakasMSFT
ms.openlocfilehash: ac0e6d67e10e7d7b81fc1c5c21e93251f84cab0a
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722555"
---
# <a name="agreementacceptance-resource-type"></a><span data-ttu-id="e6e5f-103">Tipo de recurso agreementAcceptance</span><span class="sxs-lookup"><span data-stu-id="e6e5f-103">agreementAcceptance resource type</span></span>

<span data-ttu-id="e6e5f-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e6e5f-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e6e5f-105">Representa o status atual de um usuário dentro do escopo dos termos de uso personalizáveis de uma empresa com o Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="e6e5f-105">Represents the current status of a user within scope of a company's customizable terms of use powered by Azure Active Directory (Azure AD).</span></span>

## <a name="properties"></a><span data-ttu-id="e6e5f-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="e6e5f-106">Properties</span></span>
| <span data-ttu-id="e6e5f-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e6e5f-107">Property</span></span>     | <span data-ttu-id="e6e5f-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="e6e5f-108">Type</span></span>        | <span data-ttu-id="e6e5f-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="e6e5f-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e6e5f-110">agreementFileId</span><span class="sxs-lookup"><span data-stu-id="e6e5f-110">agreementFileId</span></span>|<span data-ttu-id="e6e5f-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6e5f-111">String</span></span>|<span data-ttu-id="e6e5f-112">O identificador do arquivo de contrato aceito pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="e6e5f-112">The identifier of the agreement file accepted by the user.</span></span>|
|<span data-ttu-id="e6e5f-113">agreementId</span><span class="sxs-lookup"><span data-stu-id="e6e5f-113">agreementId</span></span>|<span data-ttu-id="e6e5f-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6e5f-114">String</span></span>|<span data-ttu-id="e6e5f-115">O identificador do contrato.</span><span class="sxs-lookup"><span data-stu-id="e6e5f-115">The identifier of the agreement.</span></span>|
|<span data-ttu-id="e6e5f-116">deviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="e6e5f-116">deviceDisplayName</span></span>|<span data-ttu-id="e6e5f-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6e5f-117">String</span></span>|<span data-ttu-id="e6e5f-118">O nome de exibição do dispositivo usado para aceitar o contrato.</span><span class="sxs-lookup"><span data-stu-id="e6e5f-118">The display name of the device used for accepting the agreement.</span></span>|
|<span data-ttu-id="e6e5f-119">deviceId</span><span class="sxs-lookup"><span data-stu-id="e6e5f-119">deviceId</span></span>|<span data-ttu-id="e6e5f-120">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6e5f-120">String</span></span>|<span data-ttu-id="e6e5f-121">O identificador exclusivo do dispositivo usado para aceitar o contrato.</span><span class="sxs-lookup"><span data-stu-id="e6e5f-121">The unique identifier of the device used for accepting the agreement.</span></span>|
|<span data-ttu-id="e6e5f-122">deviceOSType</span><span class="sxs-lookup"><span data-stu-id="e6e5f-122">deviceOSType</span></span>|<span data-ttu-id="e6e5f-123">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6e5f-123">String</span></span>|<span data-ttu-id="e6e5f-124">O sistema operacional usado para aceitar o contrato.</span><span class="sxs-lookup"><span data-stu-id="e6e5f-124">The operating system used to accept the agreement.</span></span>|
|<span data-ttu-id="e6e5f-125">deviceOSVersion</span><span class="sxs-lookup"><span data-stu-id="e6e5f-125">deviceOSVersion</span></span>|<span data-ttu-id="e6e5f-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6e5f-126">String</span></span>|<span data-ttu-id="e6e5f-127">A versão do sistema operacional do dispositivo usado para aceitar o contrato.</span><span class="sxs-lookup"><span data-stu-id="e6e5f-127">The operating system version of the device used to accept the agreement.</span></span>    |
|<span data-ttu-id="e6e5f-128">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="e6e5f-128">expirationDateTime</span></span>|<span data-ttu-id="e6e5f-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6e5f-129">DateTimeOffset</span></span>|<span data-ttu-id="e6e5f-130">A data de expiração da aceitação.</span><span class="sxs-lookup"><span data-stu-id="e6e5f-130">The expiration date time of the acceptance.</span></span> <span data-ttu-id="e6e5f-131">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="e6e5f-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="e6e5f-132">Por exemplo, meia-noite em UTC no dia 1° de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e6e5f-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e6e5f-133">id</span><span class="sxs-lookup"><span data-stu-id="e6e5f-133">id</span></span>|<span data-ttu-id="e6e5f-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6e5f-134">String</span></span>| <span data-ttu-id="e6e5f-135">O identificador da aceitação do contrato.</span><span class="sxs-lookup"><span data-stu-id="e6e5f-135">The identifier of the agreement acceptance.</span></span> <span data-ttu-id="e6e5f-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="e6e5f-136">Read-only.</span></span>|
|<span data-ttu-id="e6e5f-137">recordedDateTime</span><span class="sxs-lookup"><span data-stu-id="e6e5f-137">recordedDateTime</span></span>|<span data-ttu-id="e6e5f-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e6e5f-138">DateTimeOffset</span></span>|<span data-ttu-id="e6e5f-p103">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC. Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="e6e5f-p103">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="e6e5f-141">estado</span><span class="sxs-lookup"><span data-stu-id="e6e5f-141">state</span></span>|<span data-ttu-id="e6e5f-142">string</span><span class="sxs-lookup"><span data-stu-id="e6e5f-142">string</span></span>| <span data-ttu-id="e6e5f-143">O estado da aceitação do contrato.</span><span class="sxs-lookup"><span data-stu-id="e6e5f-143">The state of the agreement acceptance.</span></span> <span data-ttu-id="e6e5f-144">Os valores possíveis são: `accepted` e `declined`.</span><span class="sxs-lookup"><span data-stu-id="e6e5f-144">Possible values are: `accepted`, `declined`.</span></span>|
|<span data-ttu-id="e6e5f-145">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e6e5f-145">userDisplayName</span></span>|<span data-ttu-id="e6e5f-146">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6e5f-146">String</span></span>|<span data-ttu-id="e6e5f-147">Nome de exibição do usuário quando a aceitação foi registrada.</span><span class="sxs-lookup"><span data-stu-id="e6e5f-147">Display name of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="e6e5f-148">userEmail</span><span class="sxs-lookup"><span data-stu-id="e6e5f-148">userEmail</span></span>|<span data-ttu-id="e6e5f-149">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6e5f-149">String</span></span>|<span data-ttu-id="e6e5f-150">Email do usuário quando a aceitação foi registrada.</span><span class="sxs-lookup"><span data-stu-id="e6e5f-150">Email of the user when the acceptance was recorded.</span></span>|
|<span data-ttu-id="e6e5f-151">userId</span><span class="sxs-lookup"><span data-stu-id="e6e5f-151">userId</span></span>|<span data-ttu-id="e6e5f-152">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6e5f-152">String</span></span>|<span data-ttu-id="e6e5f-153">O identificador do usuário que aceitou o contrato.</span><span class="sxs-lookup"><span data-stu-id="e6e5f-153">The identifier of the user who accepted the agreement.</span></span>|
|<span data-ttu-id="e6e5f-154">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="e6e5f-154">userPrincipalName</span></span>|<span data-ttu-id="e6e5f-155">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e6e5f-155">String</span></span>|<span data-ttu-id="e6e5f-156">UPN do usuário quando a aceitação foi registrada.</span><span class="sxs-lookup"><span data-stu-id="e6e5f-156">UPN of the user when the acceptance was recorded.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e6e5f-157">Relações</span><span class="sxs-lookup"><span data-stu-id="e6e5f-157">Relationships</span></span>
<span data-ttu-id="e6e5f-158">Nenhum</span><span class="sxs-lookup"><span data-stu-id="e6e5f-158">None.</span></span>


## <a name="json-representation"></a><span data-ttu-id="e6e5f-159">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="e6e5f-159">JSON representation</span></span>

<span data-ttu-id="e6e5f-160">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="e6e5f-160">The following is a JSON representation of the resource.</span></span>

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


