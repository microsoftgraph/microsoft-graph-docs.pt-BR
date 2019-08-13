---
title: tipo de recurso windowsKioskActiveDirectoryGroup
description: A classe usada para identificar um grupo de diretórios do Azure para a configuração do quiosque
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 5451050bb70cb9cdbcc50738da0eb81c659f8e6f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371023"
---
# <a name="windowskioskactivedirectorygroup-resource-type"></a><span data-ttu-id="37330-103">tipo de recurso windowsKioskActiveDirectoryGroup</span><span class="sxs-lookup"><span data-stu-id="37330-103">windowsKioskActiveDirectoryGroup resource type</span></span>

> <span data-ttu-id="37330-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="37330-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37330-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="37330-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37330-106">A classe usada para identificar um grupo de diretórios do Azure para a configuração do quiosque</span><span class="sxs-lookup"><span data-stu-id="37330-106">The class used to identify an Azure Directory group for the kiosk configuration</span></span>


<span data-ttu-id="37330-107">Herda de [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span><span class="sxs-lookup"><span data-stu-id="37330-107">Inherits from [windowsKioskUser](../resources/intune-deviceconfig-windowskioskuser.md)</span></span>

## <a name="properties"></a><span data-ttu-id="37330-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="37330-108">Properties</span></span>
|<span data-ttu-id="37330-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="37330-109">Property</span></span>|<span data-ttu-id="37330-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="37330-110">Type</span></span>|<span data-ttu-id="37330-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="37330-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37330-112">Nome_do_grupo</span><span class="sxs-lookup"><span data-stu-id="37330-112">groupName</span></span>|<span data-ttu-id="37330-113">String</span><span class="sxs-lookup"><span data-stu-id="37330-113">String</span></span>|<span data-ttu-id="37330-114">O nome do grupo do AD que será bloqueado para esta configuração de quiosque</span><span class="sxs-lookup"><span data-stu-id="37330-114">The name of the AD group that will be locked to this kiosk configuration</span></span>|

## <a name="relationships"></a><span data-ttu-id="37330-115">Relações</span><span class="sxs-lookup"><span data-stu-id="37330-115">Relationships</span></span>
<span data-ttu-id="37330-116">Nenhum</span><span class="sxs-lookup"><span data-stu-id="37330-116">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="37330-117">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="37330-117">JSON Representation</span></span>
<span data-ttu-id="37330-118">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="37330-118">Here is a JSON representation of the resource.</span></span>
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



