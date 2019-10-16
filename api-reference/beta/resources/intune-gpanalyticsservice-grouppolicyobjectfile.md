---
title: tipo de recurso groupPolicyObjectFile
description: O arquivo de objeto da diretiva de grupo carregado por administrador.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b28ba6364f3261a7cd341870de402dc9332c87b4
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37539194"
---
# <a name="grouppolicyobjectfile-resource-type"></a><span data-ttu-id="6c5f9-103">tipo de recurso groupPolicyObjectFile</span><span class="sxs-lookup"><span data-stu-id="6c5f9-103">groupPolicyObjectFile resource type</span></span>

> <span data-ttu-id="6c5f9-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="6c5f9-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c5f9-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="6c5f9-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c5f9-106">O arquivo de objeto da diretiva de grupo carregado por administrador.</span><span class="sxs-lookup"><span data-stu-id="6c5f9-106">The Group Policy Object file uploaded by admin.</span></span>

## <a name="properties"></a><span data-ttu-id="6c5f9-107">Propriedades</span><span class="sxs-lookup"><span data-stu-id="6c5f9-107">Properties</span></span>
|<span data-ttu-id="6c5f9-108">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6c5f9-108">Property</span></span>|<span data-ttu-id="6c5f9-109">Tipo</span><span class="sxs-lookup"><span data-stu-id="6c5f9-109">Type</span></span>|<span data-ttu-id="6c5f9-110">Descrição</span><span class="sxs-lookup"><span data-stu-id="6c5f9-110">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6c5f9-111">ouDistinguishedName</span><span class="sxs-lookup"><span data-stu-id="6c5f9-111">ouDistinguishedName</span></span>|<span data-ttu-id="6c5f9-112">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c5f9-112">String</span></span>|<span data-ttu-id="6c5f9-113">O nome diferenciado da OU.</span><span class="sxs-lookup"><span data-stu-id="6c5f9-113">The distinguished name of the OU.</span></span>|
|<span data-ttu-id="6c5f9-114">content</span><span class="sxs-lookup"><span data-stu-id="6c5f9-114">content</span></span>|<span data-ttu-id="6c5f9-115">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6c5f9-115">String</span></span>|<span data-ttu-id="6c5f9-116">O conteúdo do arquivo do objeto de diretiva de grupo.</span><span class="sxs-lookup"><span data-stu-id="6c5f9-116">The Group Policy Object file content.</span></span>|

## <a name="relationships"></a><span data-ttu-id="6c5f9-117">Relações</span><span class="sxs-lookup"><span data-stu-id="6c5f9-117">Relationships</span></span>
<span data-ttu-id="6c5f9-118">Nenhum</span><span class="sxs-lookup"><span data-stu-id="6c5f9-118">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="6c5f9-119">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="6c5f9-119">JSON Representation</span></span>
<span data-ttu-id="6c5f9-120">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="6c5f9-120">Here is a JSON representation of the resource.</span></span>
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



