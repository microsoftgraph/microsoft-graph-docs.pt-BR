---
title: Tipo de recurso windowsInformationProtectionResourceCollection
description: Coleção de recursos da Proteção de Informações do Windows
ms.openlocfilehash: c6840c8ebb272d0ad066556d9edab825b3fb50f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27039653"
---
# <a name="windowsinformationprotectionresourcecollection-resource-type"></a><span data-ttu-id="180a0-103">Tipo de recurso windowsInformationProtectionResourceCollection</span><span class="sxs-lookup"><span data-stu-id="180a0-103">windowsInformationProtectionResourceCollection resource type</span></span>

> <span data-ttu-id="180a0-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="180a0-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="180a0-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="180a0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="180a0-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="180a0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="180a0-107">Coleção de recursos da Proteção de Informações do Windows</span><span class="sxs-lookup"><span data-stu-id="180a0-107">Windows Information Protection Resource Collection</span></span>
## <a name="properties"></a><span data-ttu-id="180a0-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="180a0-108">Properties</span></span>
|<span data-ttu-id="180a0-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="180a0-109">Property</span></span>|<span data-ttu-id="180a0-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="180a0-110">Type</span></span>|<span data-ttu-id="180a0-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="180a0-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="180a0-112">displayName</span><span class="sxs-lookup"><span data-stu-id="180a0-112">displayName</span></span>|<span data-ttu-id="180a0-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="180a0-113">String</span></span>|<span data-ttu-id="180a0-114">Nome de exibição</span><span class="sxs-lookup"><span data-stu-id="180a0-114">Display name</span></span>|
|<span data-ttu-id="180a0-115">recursos</span><span class="sxs-lookup"><span data-stu-id="180a0-115">resources</span></span>|<span data-ttu-id="180a0-116">String collection</span><span class="sxs-lookup"><span data-stu-id="180a0-116">String collection</span></span>|<span data-ttu-id="180a0-117">Coleção de recursos</span><span class="sxs-lookup"><span data-stu-id="180a0-117">Collection of resources</span></span>|

## <a name="relationships"></a><span data-ttu-id="180a0-118">Relações</span><span class="sxs-lookup"><span data-stu-id="180a0-118">Relationships</span></span>
<span data-ttu-id="180a0-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="180a0-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="180a0-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="180a0-120">JSON Representation</span></span>
<span data-ttu-id="180a0-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="180a0-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionResourceCollection"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionResourceCollection",
  "displayName": "String",
  "resources": [
    "String"
  ]
}
```





