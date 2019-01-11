---
title: tipo de recurso de onPremisesProvisioningError
description: Representa os erros de sincronização de diretório para o usuário, grupo ou organizacionais entidades visita quando a sincronização local diretórios no Windows Azure Active Directory.
localization_priority: Normal
ms.openlocfilehash: 1ea9efcd4d9db5cf7cc5b8f0a18b35345d06c3fe
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27817735"
---
# <a name="onpremisesprovisioningerror-resource-type"></a><span data-ttu-id="ecc3d-103">tipo de recurso de onPremisesProvisioningError</span><span class="sxs-lookup"><span data-stu-id="ecc3d-103">onPremisesProvisioningError resource type</span></span>

> <span data-ttu-id="ecc3d-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ecc3d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ecc3d-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ecc3d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ecc3d-106">Representa os erros de sincronização de diretório para as entidades de [usuário](user.md), [grupo](group.md)ou [contato organizacional](orgcontact.md) quando a sincronização local diretórios no Windows Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="ecc3d-106">Represents directory synchronization errors for the [user](user.md), [group](group.md), or [organizational contact](orgcontact.md) entities when synchronizing on-premises directories to Azure Active Directory.</span></span>

## <a name="properties"></a><span data-ttu-id="ecc3d-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ecc3d-107">Properties</span></span>

| <span data-ttu-id="ecc3d-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ecc3d-108">Property</span></span> | <span data-ttu-id="ecc3d-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="ecc3d-109">Type</span></span> | <span data-ttu-id="ecc3d-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="ecc3d-110">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="ecc3d-111">Ferramentas para desenvolvedores</span><span class="sxs-lookup"><span data-stu-id="ecc3d-111">category</span></span>|<span data-ttu-id="ecc3d-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecc3d-112">String</span></span>| <span data-ttu-id="ecc3d-113">Categoria do erro provisionamento.</span><span class="sxs-lookup"><span data-stu-id="ecc3d-113">Category of the provisioning error.</span></span> <span data-ttu-id="ecc3d-114">Observação: No momento, há apenas um valor possível.</span><span class="sxs-lookup"><span data-stu-id="ecc3d-114">Note: Currently, there is only one possible value.</span></span> <span data-ttu-id="ecc3d-115">Valores possíveis: *PropertyConflict* - indica um valor de propriedade não é exclusivo.</span><span class="sxs-lookup"><span data-stu-id="ecc3d-115">Possible value: *PropertyConflict* - indicates a property value is not unique.</span></span> <span data-ttu-id="ecc3d-116">Outros objetos contenham o mesmo valor da propriedade.</span><span class="sxs-lookup"><span data-stu-id="ecc3d-116">Other objects contain the same value for the property.</span></span> |
|<span data-ttu-id="ecc3d-117">occurredDateTime</span><span class="sxs-lookup"><span data-stu-id="ecc3d-117">occurredDateTime</span></span>|<span data-ttu-id="ecc3d-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ecc3d-118">DateTimeOffset</span></span>| <span data-ttu-id="ecc3d-119">A data e hora em que o erro ocorreu.</span><span class="sxs-lookup"><span data-stu-id="ecc3d-119">The date and time at which the error occurred.</span></span> |
|<span data-ttu-id="ecc3d-120">propertyCausingError</span><span class="sxs-lookup"><span data-stu-id="ecc3d-120">propertyCausingError</span></span>|<span data-ttu-id="ecc3d-121">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecc3d-121">String</span></span>| <span data-ttu-id="ecc3d-122">Nome da propriedade diretório que causou o erro.</span><span class="sxs-lookup"><span data-stu-id="ecc3d-122">Name of the directory property causing the error.</span></span> <span data-ttu-id="ecc3d-123">Valores possíveis atuais: *UserPrincipalName* ou *ProxyAddress*</span><span class="sxs-lookup"><span data-stu-id="ecc3d-123">Current possible values: *UserPrincipalName* or *ProxyAddress*</span></span> |
|<span data-ttu-id="ecc3d-124">valor</span><span class="sxs-lookup"><span data-stu-id="ecc3d-124">value</span></span>|<span data-ttu-id="ecc3d-125">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ecc3d-125">String</span></span>| <span data-ttu-id="ecc3d-126">Valor da propriedade que causou o erro.</span><span class="sxs-lookup"><span data-stu-id="ecc3d-126">Value of the property causing the error.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="ecc3d-127">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ecc3d-127">JSON representation</span></span>
<span data-ttu-id="ecc3d-128">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ecc3d-128">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onPremisesProvisioningError"
}-->

```json
{
  "category": "String",
  "occurredDateTime": "String (timestamp)",
  "propertyCausingError": "String",
  "value": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onPremisesProvisioningError resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
