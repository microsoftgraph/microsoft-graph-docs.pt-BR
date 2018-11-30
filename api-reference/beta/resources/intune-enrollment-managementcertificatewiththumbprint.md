---
title: tipo de recurso de managementCertificateWithThumbprint
description: Ainda não documentado
ms.openlocfilehash: 320b6241e1ac5a9078ccc32f99f87e9fd337335e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27037974"
---
# <a name="managementcertificatewiththumbprint-resource-type"></a><span data-ttu-id="1f5a3-103">tipo de recurso de managementCertificateWithThumbprint</span><span class="sxs-lookup"><span data-stu-id="1f5a3-103">managementCertificateWithThumbprint resource type</span></span>

> <span data-ttu-id="1f5a3-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="1f5a3-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f5a3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="1f5a3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1f5a3-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="1f5a3-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f5a3-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="1f5a3-107">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="1f5a3-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="1f5a3-108">Properties</span></span>
|<span data-ttu-id="1f5a3-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="1f5a3-109">Property</span></span>|<span data-ttu-id="1f5a3-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="1f5a3-110">Type</span></span>|<span data-ttu-id="1f5a3-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="1f5a3-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f5a3-112">impressão digital</span><span class="sxs-lookup"><span data-stu-id="1f5a3-112">thumbprint</span></span>|<span data-ttu-id="1f5a3-113">String</span><span class="sxs-lookup"><span data-stu-id="1f5a3-113">String</span></span>|<span data-ttu-id="1f5a3-114">A impressão digital do certificado gerenciamento</span><span class="sxs-lookup"><span data-stu-id="1f5a3-114">The thumbprint of the management certificate</span></span>|
|<span data-ttu-id="1f5a3-115">certificado</span><span class="sxs-lookup"><span data-stu-id="1f5a3-115">certificate</span></span>|<span data-ttu-id="1f5a3-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="1f5a3-116">String</span></span>|<span data-ttu-id="1f5a3-117">O certificado de gerenciamento codificada de Base 64</span><span class="sxs-lookup"><span data-stu-id="1f5a3-117">The Base 64 encoded management certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="1f5a3-118">Relações</span><span class="sxs-lookup"><span data-stu-id="1f5a3-118">Relationships</span></span>
<span data-ttu-id="1f5a3-119">Nenhum</span><span class="sxs-lookup"><span data-stu-id="1f5a3-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1f5a3-120">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="1f5a3-120">JSON Representation</span></span>
<span data-ttu-id="1f5a3-121">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="1f5a3-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.managementCertificateWithThumbprint"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managementCertificateWithThumbprint",
  "thumbprint": "String",
  "certificate": "String"
}
```





