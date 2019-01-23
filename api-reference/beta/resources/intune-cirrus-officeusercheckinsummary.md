---
title: tipo de recurso de officeUserCheckinSummary
description: Entidade que descreve as estatísticas de check-in do inquilino.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d44c978ff1442c98038bf627397de5ca3a0ca3bf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411005"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="5dc9f-103">tipo de recurso de officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="5dc9f-103">officeUserCheckinSummary resource type</span></span>

> <span data-ttu-id="5dc9f-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="5dc9f-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5dc9f-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="5dc9f-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5dc9f-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="5dc9f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5dc9f-107">Entidade que descreve as estatísticas de check-in do inquilino.</span><span class="sxs-lookup"><span data-stu-id="5dc9f-107">Entity that describes  tenant check-in stats.</span></span>

## <a name="properties"></a><span data-ttu-id="5dc9f-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="5dc9f-108">Properties</span></span>
|<span data-ttu-id="5dc9f-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="5dc9f-109">Property</span></span>|<span data-ttu-id="5dc9f-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="5dc9f-110">Type</span></span>|<span data-ttu-id="5dc9f-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="5dc9f-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dc9f-112">succeededUserCount</span><span class="sxs-lookup"><span data-stu-id="5dc9f-112">succeededUserCount</span></span>|<span data-ttu-id="5dc9f-113">Int32</span><span class="sxs-lookup"><span data-stu-id="5dc9f-113">Int32</span></span>|<span data-ttu-id="5dc9f-114">Total de usuários bem-sucedida verificar ins nos últimos 3 meses.</span><span class="sxs-lookup"><span data-stu-id="5dc9f-114">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="5dc9f-115">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="5dc9f-115">failedUserCount</span></span>|<span data-ttu-id="5dc9f-116">Int32</span><span class="sxs-lookup"><span data-stu-id="5dc9f-116">Int32</span></span>|<span data-ttu-id="5dc9f-117">Total de usuários com falha verificar ins nos últimos 3 meses.</span><span class="sxs-lookup"><span data-stu-id="5dc9f-117">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5dc9f-118">Relações</span><span class="sxs-lookup"><span data-stu-id="5dc9f-118">Relationships</span></span>
<span data-ttu-id="5dc9f-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="5dc9f-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5dc9f-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="5dc9f-120">JSON Representation</span></span>
<span data-ttu-id="5dc9f-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="5dc9f-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.officeUserCheckinSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.officeUserCheckinSummary",
  "succeededUserCount": 1024,
  "failedUserCount": 1024
}
```



