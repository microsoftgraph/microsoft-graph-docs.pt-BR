---
title: tipo de recurso userCredentialUsageDetails
description: Representa o uso de redefinição de senha de autoatendimento para um determinado locatário.
localization_priority: Normal
author: davidmu1
ms.prod: reports
doc_type: resourcePageType
ms.openlocfilehash: bb92f3bfc91e8fa418d6a33ad6a77a5fddbf9f10
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/02/2019
ms.locfileid: "35519207"
---
# <a name="usercredentialusagedetails-resource-type"></a><span data-ttu-id="34fbe-103">tipo de recurso userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="34fbe-103">userCredentialUsageDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="34fbe-104">Representa o uso de redefinição de senha de autoatendimento para um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="34fbe-104">Represents the self-service password reset usage for a given tenant.</span></span> <span data-ttu-id="34fbe-105">Os detalhes incluem informações do usuário, status da redefinição e o motivo da falha.</span><span class="sxs-lookup"><span data-stu-id="34fbe-105">Details include user information, status of the reset, and the reason for failure.</span></span>

## <a name="methods"></a><span data-ttu-id="34fbe-106">Métodos</span><span class="sxs-lookup"><span data-stu-id="34fbe-106">Methods</span></span>

| <span data-ttu-id="34fbe-107">Método</span><span class="sxs-lookup"><span data-stu-id="34fbe-107">Method</span></span>       | <span data-ttu-id="34fbe-108">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="34fbe-108">Return Type</span></span> | <span data-ttu-id="34fbe-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="34fbe-109">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="34fbe-110">Listar userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="34fbe-110">List userCredentialUsageDetails</span></span>](../api/reportroot-list-usercredentialusagedetails.md) | <span data-ttu-id="34fbe-111">userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="34fbe-111">userCredentialUsageDetails</span></span> | <span data-ttu-id="34fbe-112">Ler propriedades e relações de um objeto userCredentialUsageDetails.</span><span class="sxs-lookup"><span data-stu-id="34fbe-112">Read properties and relationships of a userCredentialUsageDetails object.</span></span> |

## <a name="properties"></a><span data-ttu-id="34fbe-113">Propriedades</span><span class="sxs-lookup"><span data-stu-id="34fbe-113">Properties</span></span>

| <span data-ttu-id="34fbe-114">Propriedade</span><span class="sxs-lookup"><span data-stu-id="34fbe-114">Property</span></span>     | <span data-ttu-id="34fbe-115">Tipo</span><span class="sxs-lookup"><span data-stu-id="34fbe-115">Type</span></span>        | <span data-ttu-id="34fbe-116">Descrição</span><span class="sxs-lookup"><span data-stu-id="34fbe-116">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="34fbe-117">authMethod</span><span class="sxs-lookup"><span data-stu-id="34fbe-117">authMethod</span></span> | <span data-ttu-id="34fbe-118">string</span><span class="sxs-lookup"><span data-stu-id="34fbe-118">string</span></span> | <span data-ttu-id="34fbe-119">Representa o método de autenticação usado pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="34fbe-119">Represents the authentication method that the user used.</span></span> <span data-ttu-id="34fbe-120">Os valores possíveis são `email`: `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` , (usado somente para redefinição de senha de autoatendimento `appCode`), `alternateMobileCall` `appNotification`e (somente para o registro).</span><span class="sxs-lookup"><span data-stu-id="34fbe-120">Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and `alternateMobileCall` (supported only in registration).</span></span> |
| <span data-ttu-id="34fbe-121">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="34fbe-121">eventDateTime</span></span> | <span data-ttu-id="34fbe-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="34fbe-122">DateTimeOffset</span></span> | <span data-ttu-id="34fbe-123">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="34fbe-123">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="34fbe-124">Por exemplo, meia-noite em UTC no dia 1º de janeiro de 2014 teria esta aparência: `'2014-01-01T00:00:00Z'`.</span><span class="sxs-lookup"><span data-stu-id="34fbe-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> |
| <span data-ttu-id="34fbe-125">failureReason</span><span class="sxs-lookup"><span data-stu-id="34fbe-125">failureReason</span></span> | <span data-ttu-id="34fbe-126">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="34fbe-126">String</span></span> | <span data-ttu-id="34fbe-127">Fornece o motivo da falha para o fluxo de trabalho de redefinição ou registro correspondente.</span><span class="sxs-lookup"><span data-stu-id="34fbe-127">Provides the failure reason for the corresponding reset or registration workflow.</span></span> |
| <span data-ttu-id="34fbe-128">apresentam</span><span class="sxs-lookup"><span data-stu-id="34fbe-128">feature</span></span> | <span data-ttu-id="34fbe-129">string</span><span class="sxs-lookup"><span data-stu-id="34fbe-129">string</span></span> | <span data-ttu-id="34fbe-130">Os valores possíveis são `registration` : `reset`e.</span><span class="sxs-lookup"><span data-stu-id="34fbe-130">Possible values are: `registration` and `reset`.</span></span> |
| <span data-ttu-id="34fbe-131">id</span><span class="sxs-lookup"><span data-stu-id="34fbe-131">id</span></span> | <span data-ttu-id="34fbe-132">String</span><span class="sxs-lookup"><span data-stu-id="34fbe-132">String</span></span> | <span data-ttu-id="34fbe-133">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="34fbe-133">Read-only.</span></span> <span data-ttu-id="34fbe-134">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="34fbe-134">The unique identifier for the activity.</span></span> <span data-ttu-id="34fbe-135">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="34fbe-135">Read-only.</span></span>|
| <span data-ttu-id="34fbe-136">IsSuccess</span><span class="sxs-lookup"><span data-stu-id="34fbe-136">isSuccess</span></span> | <span data-ttu-id="34fbe-137">Booliano</span><span class="sxs-lookup"><span data-stu-id="34fbe-137">Boolean</span></span> | <span data-ttu-id="34fbe-138">Indica êxito ou falha do fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="34fbe-138">Indicates success or failure of the workflow.</span></span> |
| <span data-ttu-id="34fbe-139">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="34fbe-139">userDisplayName</span></span> | <span data-ttu-id="34fbe-140">String</span><span class="sxs-lookup"><span data-stu-id="34fbe-140">String</span></span> | <span data-ttu-id="34fbe-141">Nome de usuário do usuário que está executando o fluxo de trabalho de redefinição ou registro.</span><span class="sxs-lookup"><span data-stu-id="34fbe-141">User name of the user performing the reset or registration workflow.</span></span> |
| <span data-ttu-id="34fbe-142">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="34fbe-142">userPrincipalName</span></span> | <span data-ttu-id="34fbe-143">String</span><span class="sxs-lookup"><span data-stu-id="34fbe-143">String</span></span> | <span data-ttu-id="34fbe-144">Nome principal do usuário que está executando o fluxo de trabalho de redefinição ou registro.</span><span class="sxs-lookup"><span data-stu-id="34fbe-144">User principal name of the user performing the reset or registration workflow.</span></span> |

## <a name="relationships"></a><span data-ttu-id="34fbe-145">Relações</span><span class="sxs-lookup"><span data-stu-id="34fbe-145">Relationships</span></span>

<span data-ttu-id="34fbe-146">Nenhum</span><span class="sxs-lookup"><span data-stu-id="34fbe-146">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="34fbe-147">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="34fbe-147">JSON representation</span></span>

<span data-ttu-id="34fbe-148">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="34fbe-148">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userCredentialUsageDetails",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "id" : "String",
  "feature":"string",
  "userPrincipalName":"String",
  "userDisplayName": "String",
  "isSuccess" : true,
  "authMethod": "string",
  "failureReason": "String",
  "eventDateTime" : "DateTimeOffset"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "userCredentialUsageDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->