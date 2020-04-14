---
title: tipo de recurso windowsKioskActiveDirectoryGroup
description: A classe usada para identificar um grupo de diretórios do Azure para a configuração do quiosque
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: c46d3b44c28c7f07b5d0478acc3f82547b3819ee
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43466857"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="ea742-103">tipo de recurso windowsKioskActiveDirectoryGroup</span><span class="sxs-lookup"><span data-stu-id="ea742-103">windowsKioskActiveDirectoryGroup resource type</span></span>

<span data-ttu-id="ea742-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ea742-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ea742-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="ea742-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ea742-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="ea742-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ea742-107">A classe usada para identificar um grupo de diretórios do Azure para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="ea742-107">The class used to identify an Azure Directory group for the kiosk configuration</span></span>


<span data-ttu-id="ea742-108">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="ea742-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="ea742-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="ea742-109">Properties</span></span>
|<span data-ttu-id="ea742-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ea742-110">Property</span></span>|<span data-ttu-id="ea742-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="ea742-111">Type</span></span>|<span data-ttu-id="ea742-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="ea742-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ea742-113">Nome_do_grupo</span><span class="sxs-lookup"><span data-stu-id="ea742-113">groupName</span></span>|<span data-ttu-id="ea742-114">String</span><span class="sxs-lookup"><span data-stu-id="ea742-114">String</span></span>|<span data-ttu-id="ea742-115">O nome do grupo do AD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="ea742-115">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="ea742-116">Relações</span><span class="sxs-lookup"><span data-stu-id="ea742-116">Relationships</span></span>
<span data-ttu-id="ea742-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="ea742-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="ea742-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="ea742-118">JSON Representation</span></span>
<span data-ttu-id="ea742-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="ea742-119">Here is a JSON representation of the resource.</span></span>
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



