---
title: Tipo de recurso androidMobileAppIdentifier
description: O identificador de um app Android.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: f6c26c41ffcb36ee325f5e0fae907916a418fb8b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29410277"
---
# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="d88bf-103">Tipo de recurso androidMobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d88bf-103">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="d88bf-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="d88bf-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d88bf-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="d88bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d88bf-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="d88bf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d88bf-107">O identificador de um app Android.</span><span class="sxs-lookup"><span data-stu-id="d88bf-107">The identifier for an Android app.</span></span>


<span data-ttu-id="d88bf-108">Herda de [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span><span class="sxs-lookup"><span data-stu-id="d88bf-108">Inherits from [mobileAppIdentifier](../resources/intune-mam-mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d88bf-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="d88bf-109">Properties</span></span>
|<span data-ttu-id="d88bf-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="d88bf-110">Property</span></span>|<span data-ttu-id="d88bf-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="d88bf-111">Type</span></span>|<span data-ttu-id="d88bf-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="d88bf-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d88bf-113">packageId</span><span class="sxs-lookup"><span data-stu-id="d88bf-113">packageId</span></span>|<span data-ttu-id="d88bf-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="d88bf-114">String</span></span>|<span data-ttu-id="d88bf-115">O identificador de um app, como especificado na Play Store.</span><span class="sxs-lookup"><span data-stu-id="d88bf-115">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d88bf-116">Relações</span><span class="sxs-lookup"><span data-stu-id="d88bf-116">Relationships</span></span>
<span data-ttu-id="d88bf-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="d88bf-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d88bf-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="d88bf-118">JSON Representation</span></span>
<span data-ttu-id="d88bf-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="d88bf-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMobileAppIdentifier",
  "packageId": "String"
}
```




