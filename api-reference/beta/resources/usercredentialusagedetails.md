---
title: Tipo de recurso userCredentialUsageDetails
description: Representa o uso de redefinição de senha de autoatendados para um determinado locatário.
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: a10d262444b0a33dfbeadbb21611d914d9253e0d
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/11/2021
ms.locfileid: "50719903"
---
# <a name="usercredentialusagedetails-resource-type"></a><span data-ttu-id="a88ac-103">Tipo de recurso userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="a88ac-103">userCredentialUsageDetails resource type</span></span>

<span data-ttu-id="a88ac-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a88ac-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a88ac-105">Representa o uso de redefinição de senha de autoatendados para um determinado locatário.</span><span class="sxs-lookup"><span data-stu-id="a88ac-105">Represents the self-service password reset usage for a given tenant.</span></span> <span data-ttu-id="a88ac-106">Os detalhes incluem informações do usuário, status da redefinição e o motivo da falha.</span><span class="sxs-lookup"><span data-stu-id="a88ac-106">Details include user information, status of the reset, and the reason for failure.</span></span>

## <a name="methods"></a><span data-ttu-id="a88ac-107">Métodos</span><span class="sxs-lookup"><span data-stu-id="a88ac-107">Methods</span></span>

| <span data-ttu-id="a88ac-108">Método</span><span class="sxs-lookup"><span data-stu-id="a88ac-108">Method</span></span>       | <span data-ttu-id="a88ac-109">Tipo de retorno</span><span class="sxs-lookup"><span data-stu-id="a88ac-109">Return Type</span></span> | <span data-ttu-id="a88ac-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="a88ac-110">Description</span></span> |
|:-------------|:------------|:------------|
| [<span data-ttu-id="a88ac-111">Listar userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="a88ac-111">List userCredentialUsageDetails</span></span>](../api/reportroot-list-usercredentialusagedetails.md) | <span data-ttu-id="a88ac-112">userCredentialUsageDetails</span><span class="sxs-lookup"><span data-stu-id="a88ac-112">userCredentialUsageDetails</span></span> | <span data-ttu-id="a88ac-113">Ler propriedades e relações de um objeto userCredentialUsageDetails.</span><span class="sxs-lookup"><span data-stu-id="a88ac-113">Read properties and relationships of a userCredentialUsageDetails object.</span></span> |

## <a name="properties"></a><span data-ttu-id="a88ac-114">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a88ac-114">Properties</span></span>

| <span data-ttu-id="a88ac-115">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a88ac-115">Property</span></span>     | <span data-ttu-id="a88ac-116">Tipo</span><span class="sxs-lookup"><span data-stu-id="a88ac-116">Type</span></span>        | <span data-ttu-id="a88ac-117">Descrição</span><span class="sxs-lookup"><span data-stu-id="a88ac-117">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="a88ac-118">authMethod</span><span class="sxs-lookup"><span data-stu-id="a88ac-118">authMethod</span></span> | <span data-ttu-id="a88ac-119">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a88ac-119">string</span></span> | <span data-ttu-id="a88ac-120">Representa o método de autenticação que o usuário usou.</span><span class="sxs-lookup"><span data-stu-id="a88ac-120">Represents the authentication method that the user used.</span></span> <span data-ttu-id="a88ac-121">Os valores possíveis são: , , , , , (usado somente para redefinição de senha de `email` `mobileSMS` `mobileCall` `officePhone` `securityQuestion` autoatendido), `appNotification` `appCode` , e `alternateMobileCall` (suportado somente no registro).</span><span class="sxs-lookup"><span data-stu-id="a88ac-121">Possible values are: `email`, `mobileSMS`, `mobileCall`, `officePhone`, `securityQuestion` (only used for self-service password reset), `appNotification`, `appCode`, and `alternateMobileCall` (supported only in registration).</span></span> |
| <span data-ttu-id="a88ac-122">eventDateTime</span><span class="sxs-lookup"><span data-stu-id="a88ac-122">eventDateTime</span></span> | <span data-ttu-id="a88ac-123">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a88ac-123">DateTimeOffset</span></span> | <span data-ttu-id="a88ac-124">O tipo Timestamp representa informações de data e hora usando o formato ISO 8601 e está sempre no horário UTC.</span><span class="sxs-lookup"><span data-stu-id="a88ac-124">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="a88ac-125">Por exemplo, meia-noite UTC em 1 de janeiro de 2014 é `2014-01-01T00:00:00Z`.</span><span class="sxs-lookup"><span data-stu-id="a88ac-125">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> |
| <span data-ttu-id="a88ac-126">failureReason</span><span class="sxs-lookup"><span data-stu-id="a88ac-126">failureReason</span></span> | <span data-ttu-id="a88ac-127">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a88ac-127">String</span></span> | <span data-ttu-id="a88ac-128">Fornece o motivo da falha para o fluxo de trabalho de redefinição ou registro correspondente.</span><span class="sxs-lookup"><span data-stu-id="a88ac-128">Provides the failure reason for the corresponding reset or registration workflow.</span></span> |
| <span data-ttu-id="a88ac-129">feature</span><span class="sxs-lookup"><span data-stu-id="a88ac-129">feature</span></span> | <span data-ttu-id="a88ac-130">cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a88ac-130">string</span></span> | <span data-ttu-id="a88ac-131">Os valores possíveis são: `registration` e `reset` .</span><span class="sxs-lookup"><span data-stu-id="a88ac-131">Possible values are: `registration` and `reset`.</span></span> |
| <span data-ttu-id="a88ac-132">id</span><span class="sxs-lookup"><span data-stu-id="a88ac-132">id</span></span> | <span data-ttu-id="a88ac-133">String</span><span class="sxs-lookup"><span data-stu-id="a88ac-133">String</span></span> | <span data-ttu-id="a88ac-134">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a88ac-134">Read-only.</span></span> <span data-ttu-id="a88ac-135">O identificador exclusivo da atividade.</span><span class="sxs-lookup"><span data-stu-id="a88ac-135">The unique identifier for the activity.</span></span> <span data-ttu-id="a88ac-136">Somente leitura.</span><span class="sxs-lookup"><span data-stu-id="a88ac-136">Read-only.</span></span>|
| <span data-ttu-id="a88ac-137">isSuccess</span><span class="sxs-lookup"><span data-stu-id="a88ac-137">isSuccess</span></span> | <span data-ttu-id="a88ac-138">Booliano</span><span class="sxs-lookup"><span data-stu-id="a88ac-138">Boolean</span></span> | <span data-ttu-id="a88ac-139">Indica sucesso ou falha do fluxo de trabalho.</span><span class="sxs-lookup"><span data-stu-id="a88ac-139">Indicates success or failure of the workflow.</span></span> |
| <span data-ttu-id="a88ac-140">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="a88ac-140">userDisplayName</span></span> | <span data-ttu-id="a88ac-141">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a88ac-141">String</span></span> | <span data-ttu-id="a88ac-142">Nome de usuário do usuário que executa o fluxo de trabalho de redefinição ou registro.</span><span class="sxs-lookup"><span data-stu-id="a88ac-142">User name of the user performing the reset or registration workflow.</span></span> |
| <span data-ttu-id="a88ac-143">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="a88ac-143">userPrincipalName</span></span> | <span data-ttu-id="a88ac-144">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a88ac-144">String</span></span> | <span data-ttu-id="a88ac-145">Nome principal do usuário que executa o fluxo de trabalho de redefinição ou registro.</span><span class="sxs-lookup"><span data-stu-id="a88ac-145">User principal name of the user performing the reset or registration workflow.</span></span> |

## <a name="relationships"></a><span data-ttu-id="a88ac-146">Relações</span><span class="sxs-lookup"><span data-stu-id="a88ac-146">Relationships</span></span>

<span data-ttu-id="a88ac-147">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a88ac-147">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a88ac-148">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a88ac-148">JSON representation</span></span>

<span data-ttu-id="a88ac-149">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a88ac-149">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.userCredentialUsageDetails",
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

