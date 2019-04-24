---
title: tipo de recurso windowsKioskActiveDirectoryGroup
description: A classe usada para identificar um grupo de diretórios do Azure para a configuração do quiosque
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 20f4c0eaf8470f01619a9ff4067bec0d95851b3c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/24/2019
ms.locfileid: "32464621"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="a0e06-103">tipo de recurso windowsKioskActiveDirectoryGroup</span><span class="sxs-lookup"><span data-stu-id="a0e06-103">windowsKioskActiveDirectoryGroup resource type</span></span>

> <span data-ttu-id="a0e06-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="a0e06-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a0e06-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a0e06-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a0e06-106">A classe usada para identificar um grupo de diretórios do Azure para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="a0e06-106">The class used to identify an Azure Directory group for the kiosk configuration</span></span>


<span data-ttu-id="a0e06-107">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="a0e06-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a0e06-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0e06-108">Properties</span></span>
|<span data-ttu-id="a0e06-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0e06-109">Property</span></span>|<span data-ttu-id="a0e06-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0e06-110">Type</span></span>|<span data-ttu-id="a0e06-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0e06-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0e06-112">Nome_do_grupo</span><span class="sxs-lookup"><span data-stu-id="a0e06-112">groupName</span></span>|<span data-ttu-id="a0e06-113">String</span><span class="sxs-lookup"><span data-stu-id="a0e06-113">String</span></span>|<span data-ttu-id="a0e06-114">O nome do grupo do AD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="a0e06-114">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0e06-115">Relações</span><span class="sxs-lookup"><span data-stu-id="a0e06-115">Relationships</span></span>
<span data-ttu-id="a0e06-116">Nenhuma</span><span class="sxs-lookup"><span data-stu-id="a0e06-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="a0e06-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0e06-117">JSON Representation</span></span>
<span data-ttu-id="a0e06-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a0e06-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsKioskActiveDirectoryGroup"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsKioskActiveDirectoryGroup",
  "groupName": "String"
}
```





