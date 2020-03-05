---
title: tipo de recurso windowsKioskActiveDirectoryGroup
description: A classe usada para identificar um grupo de diretórios do Azure para a configuração do quiosque
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ab2a9834e4f3eac6fbff84fc84a78873aca8415f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42529059"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="20792-103">tipo de recurso windowsKioskActiveDirectoryGroup</span><span class="sxs-lookup"><span data-stu-id="20792-103">windowsKioskActiveDirectoryGroup resource type</span></span>

<span data-ttu-id="20792-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="20792-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="20792-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="20792-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20792-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="20792-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20792-107">A classe usada para identificar um grupo de diretórios do Azure para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="20792-107">The class used to identify an Azure Directory group for the kiosk configuration</span></span>


<span data-ttu-id="20792-108">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="20792-108">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="20792-109">Propriedades</span><span class="sxs-lookup"><span data-stu-id="20792-109">Properties</span></span>
|<span data-ttu-id="20792-110">Propriedade</span><span class="sxs-lookup"><span data-stu-id="20792-110">Property</span></span>|<span data-ttu-id="20792-111">Tipo</span><span class="sxs-lookup"><span data-stu-id="20792-111">Type</span></span>|<span data-ttu-id="20792-112">Descrição</span><span class="sxs-lookup"><span data-stu-id="20792-112">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20792-113">Nome_do_grupo</span><span class="sxs-lookup"><span data-stu-id="20792-113">groupName</span></span>|<span data-ttu-id="20792-114">String</span><span class="sxs-lookup"><span data-stu-id="20792-114">String</span></span>|<span data-ttu-id="20792-115">O nome do grupo do AD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="20792-115">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="20792-116">Relações</span><span class="sxs-lookup"><span data-stu-id="20792-116">Relationships</span></span>
<span data-ttu-id="20792-117">Nenhum</span><span class="sxs-lookup"><span data-stu-id="20792-117">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="20792-118">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="20792-118">JSON Representation</span></span>
<span data-ttu-id="20792-119">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="20792-119">Here is a JSON representation of the resource.</span></span>
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



