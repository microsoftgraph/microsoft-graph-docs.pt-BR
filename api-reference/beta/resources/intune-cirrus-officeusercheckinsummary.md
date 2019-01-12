---
title: tipo de recurso de officeUserCheckinSummary
description: Entidade que descreve as estatísticas de check-in do inquilino.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 374f5113a517b52ae7af6381f575ac60e5d00ae4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946578"
---
# <a name="officeusercheckinsummary-resource-type"></a><span data-ttu-id="96b18-103">tipo de recurso de officeUserCheckinSummary</span><span class="sxs-lookup"><span data-stu-id="96b18-103">officeUserCheckinSummary resource type</span></span>

> <span data-ttu-id="96b18-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="96b18-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="96b18-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="96b18-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="96b18-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="96b18-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="96b18-107">Entidade que descreve as estatísticas de check-in do inquilino.</span><span class="sxs-lookup"><span data-stu-id="96b18-107">Entity that describes  tenant check-in stats.</span></span>
## <a name="properties"></a><span data-ttu-id="96b18-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="96b18-108">Properties</span></span>
|<span data-ttu-id="96b18-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="96b18-109">Property</span></span>|<span data-ttu-id="96b18-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="96b18-110">Type</span></span>|<span data-ttu-id="96b18-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="96b18-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96b18-112">succeededUserCount</span><span class="sxs-lookup"><span data-stu-id="96b18-112">succeededUserCount</span></span>|<span data-ttu-id="96b18-113">Int32</span><span class="sxs-lookup"><span data-stu-id="96b18-113">Int32</span></span>|<span data-ttu-id="96b18-114">Total de usuários bem-sucedida verificar ins nos últimos 3 meses.</span><span class="sxs-lookup"><span data-stu-id="96b18-114">Total successful user check ins for the last 3 months.</span></span>|
|<span data-ttu-id="96b18-115">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="96b18-115">failedUserCount</span></span>|<span data-ttu-id="96b18-116">Int32</span><span class="sxs-lookup"><span data-stu-id="96b18-116">Int32</span></span>|<span data-ttu-id="96b18-117">Total de usuários com falha verificar ins nos últimos 3 meses.</span><span class="sxs-lookup"><span data-stu-id="96b18-117">Total failed user check ins for the last 3 months.</span></span>|

## <a name="relationships"></a><span data-ttu-id="96b18-118">Relações</span><span class="sxs-lookup"><span data-stu-id="96b18-118">Relationships</span></span>
<span data-ttu-id="96b18-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="96b18-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="96b18-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="96b18-120">JSON Representation</span></span>
<span data-ttu-id="96b18-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="96b18-121">Here is a JSON representation of the resource.</span></span>
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



