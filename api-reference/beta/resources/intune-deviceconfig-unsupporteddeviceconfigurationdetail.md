---
title: tipo de recurso de unsupportedDeviceConfigurationDetail
description: Uma descrição por que não há suporte para uma entidade.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0a213961e6b816917b061bc56c792cf9a60e3a2a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839470"
---
# <a name="unsupporteddeviceconfigurationdetail-resource-type"></a><span data-ttu-id="c2773-103">tipo de recurso de unsupportedDeviceConfigurationDetail</span><span class="sxs-lookup"><span data-stu-id="c2773-103">unsupportedDeviceConfigurationDetail resource type</span></span>

> <span data-ttu-id="c2773-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="c2773-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c2773-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="c2773-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c2773-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="c2773-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c2773-107">Uma descrição por que não há suporte para uma entidade.</span><span class="sxs-lookup"><span data-stu-id="c2773-107">A description of why an entity is unsupported.</span></span>
## <a name="properties"></a><span data-ttu-id="c2773-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="c2773-108">Properties</span></span>
|<span data-ttu-id="c2773-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="c2773-109">Property</span></span>|<span data-ttu-id="c2773-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="c2773-110">Type</span></span>|<span data-ttu-id="c2773-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="c2773-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2773-112">mensagem</span><span class="sxs-lookup"><span data-stu-id="c2773-112">message</span></span>|<span data-ttu-id="c2773-113">String</span><span class="sxs-lookup"><span data-stu-id="c2773-113">String</span></span>|<span data-ttu-id="c2773-114">Uma mensagem que explica por que não há suporte para uma entidade.</span><span class="sxs-lookup"><span data-stu-id="c2773-114">A message explaining why an entity is unsupported.</span></span>|
|<span data-ttu-id="c2773-115">propertyName</span><span class="sxs-lookup"><span data-stu-id="c2773-115">propertyName</span></span>|<span data-ttu-id="c2773-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="c2773-116">String</span></span>|<span data-ttu-id="c2773-117">Se a mensagem está relacionada a uma propriedade específica à entidade original e, em seguida, o nome dessa propriedade.</span><span class="sxs-lookup"><span data-stu-id="c2773-117">If message is related to a specific property in the original entity, then the name of that property.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c2773-118">Relações</span><span class="sxs-lookup"><span data-stu-id="c2773-118">Relationships</span></span>
<span data-ttu-id="c2773-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="c2773-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c2773-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="c2773-120">JSON Representation</span></span>
<span data-ttu-id="c2773-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="c2773-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.unsupportedDeviceConfigurationDetail"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.unsupportedDeviceConfigurationDetail",
  "message": "String",
  "propertyName": "String"
}
```





