---
title: tipo de recurso groupPolicyObjectFile
description: O arquivo de objeto da diretiva de grupo carregado por administrador.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 26881a87b7f22510acf760ae04f967db021e8730
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42524473"
---
# <a name="grouppolicyobjectfile-resource-type"></a><span data-ttu-id="35a87-103">tipo de recurso groupPolicyObjectFile</span><span class="sxs-lookup"><span data-stu-id="35a87-103">groupPolicyObjectFile resource type</span></span>

<span data-ttu-id="35a87-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="35a87-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="35a87-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="35a87-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="35a87-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="35a87-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="35a87-107">O arquivo de objeto da diretiva de grupo carregado por administrador.</span><span class="sxs-lookup"><span data-stu-id="35a87-107">The Group Policy Object file uploaded by admin.</span></span>

## <a name="properties"></a><span data-ttu-id="35a87-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="35a87-108">Properties</span></span>
|<span data-ttu-id="35a87-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="35a87-109">Property</span></span>|<span data-ttu-id="35a87-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="35a87-110">Type</span></span>|<span data-ttu-id="35a87-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="35a87-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35a87-112">ouDistinguishedName</span><span class="sxs-lookup"><span data-stu-id="35a87-112">ouDistinguishedName</span></span>|<span data-ttu-id="35a87-113">String</span><span class="sxs-lookup"><span data-stu-id="35a87-113">String</span></span>|<span data-ttu-id="35a87-114">O nome diferenciado da OU.</span><span class="sxs-lookup"><span data-stu-id="35a87-114">The distinguished name of the OU.</span></span>|
|<span data-ttu-id="35a87-115">content</span><span class="sxs-lookup"><span data-stu-id="35a87-115">content</span></span>|<span data-ttu-id="35a87-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="35a87-116">String</span></span>|<span data-ttu-id="35a87-117">O conteúdo do arquivo do objeto de diretiva de grupo.</span><span class="sxs-lookup"><span data-stu-id="35a87-117">The Group Policy Object file content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="35a87-118">Relações</span><span class="sxs-lookup"><span data-stu-id="35a87-118">Relationships</span></span>
<span data-ttu-id="35a87-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="35a87-119">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="35a87-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="35a87-120">JSON Representation</span></span>
<span data-ttu-id="35a87-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="35a87-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.groupPolicyObjectFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyObjectFile",
  "ouDistinguishedName": "String",
  "content": "String"
}
```



