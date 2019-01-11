---
title: tipo de recurso de customSubjectAlternativeName
description: Definição de nome alternativo da entidade personalizada
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b8f0587e74e9c059ca3cbbda6af6947ded3b6bce
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27841129"
---
# <a name="customsubjectalternativename-resource-type"></a><span data-ttu-id="15c32-103">tipo de recurso de customSubjectAlternativeName</span><span class="sxs-lookup"><span data-stu-id="15c32-103">customSubjectAlternativeName resource type</span></span>

> <span data-ttu-id="15c32-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="15c32-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15c32-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="15c32-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15c32-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="15c32-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15c32-107">Definição de nome alternativo da entidade personalizada</span><span class="sxs-lookup"><span data-stu-id="15c32-107">Custom Subject Alternative Name definition</span></span>
## <a name="properties"></a><span data-ttu-id="15c32-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="15c32-108">Properties</span></span>
|<span data-ttu-id="15c32-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="15c32-109">Property</span></span>|<span data-ttu-id="15c32-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="15c32-110">Type</span></span>|<span data-ttu-id="15c32-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="15c32-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15c32-112">sanType</span><span class="sxs-lookup"><span data-stu-id="15c32-112">sanType</span></span>|[<span data-ttu-id="15c32-113">subjectAlternativeNameType</span><span class="sxs-lookup"><span data-stu-id="15c32-113">subjectAlternativeNameType</span></span>](../resources/intune-deviceconfig-subjectalternativenametype.md)|<span data-ttu-id="15c32-114">Tipo de SAN personalizado.</span><span class="sxs-lookup"><span data-stu-id="15c32-114">Custom SAN Type.</span></span> <span data-ttu-id="15c32-115">Os valores possíveis são: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span><span class="sxs-lookup"><span data-stu-id="15c32-115">Possible values are: `none`, `emailAddress`, `userPrincipalName`, `customAzureADAttribute`, `domainNameService`.</span></span>|
|<span data-ttu-id="15c32-116">name</span><span class="sxs-lookup"><span data-stu-id="15c32-116">name</span></span>|<span data-ttu-id="15c32-117">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="15c32-117">String</span></span>|<span data-ttu-id="15c32-118">Nome de SAN personalizado</span><span class="sxs-lookup"><span data-stu-id="15c32-118">Custom SAN Name</span></span>|

## <a name="relationships"></a><span data-ttu-id="15c32-119">Relações</span><span class="sxs-lookup"><span data-stu-id="15c32-119">Relationships</span></span>
<span data-ttu-id="15c32-120">Nenhum</span><span class="sxs-lookup"><span data-stu-id="15c32-120">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="15c32-121">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="15c32-121">JSON Representation</span></span>
<span data-ttu-id="15c32-122">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="15c32-122">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.customSubjectAlternativeName"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.customSubjectAlternativeName",
  "sanType": "String",
  "name": "String"
}
```





