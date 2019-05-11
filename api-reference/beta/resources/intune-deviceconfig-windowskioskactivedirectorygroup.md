---
title: tipo de recurso windowsKioskActiveDirectoryGroup
description: A classe usada para identificar um grupo de diretórios do Azure para a configuração do quiosque
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: d4c0810cfeda4f620f6733a5b824cde8d0234f38
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 05/11/2019
ms.locfileid: "33943960"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="67647-103">tipo de recurso windowsKioskActiveDirectoryGroup</span><span class="sxs-lookup"><span data-stu-id="67647-103">windowsKioskActiveDirectoryGroup resource type</span></span>

> <span data-ttu-id="67647-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="67647-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67647-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="67647-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67647-106">A classe usada para identificar um grupo de diretórios do Azure para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="67647-106">The class used to identify an Azure Directory group for the kiosk configuration</span></span>


<span data-ttu-id="67647-107">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="67647-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="67647-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="67647-108">Properties</span></span>
|<span data-ttu-id="67647-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="67647-109">Property</span></span>|<span data-ttu-id="67647-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="67647-110">Type</span></span>|<span data-ttu-id="67647-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="67647-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67647-112">Nome_do_grupo</span><span class="sxs-lookup"><span data-stu-id="67647-112">groupName</span></span>|<span data-ttu-id="67647-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="67647-113">String</span></span>|<span data-ttu-id="67647-114">O nome do grupo do AD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="67647-114">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="67647-115">Relações</span><span class="sxs-lookup"><span data-stu-id="67647-115">Relationships</span></span>
<span data-ttu-id="67647-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="67647-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="67647-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="67647-117">JSON Representation</span></span>
<span data-ttu-id="67647-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="67647-118">Here is a JSON representation of the resource.</span></span>
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




