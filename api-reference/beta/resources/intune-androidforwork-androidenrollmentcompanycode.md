---
title: tipo de recurso androidEnrollmentCompanyCode
description: Uma classe para manter os dados de registro Specialty usados para registrar-se por meio da API de gerenciamento do Android do Google, como token, URL e conteúdo de código QR
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b380ea8b085b0328b166b6f9ba0f65bf5df4af76
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43459288"
---
# <a name="androidenrollmentcompanycode-resource-type"></a><span data-ttu-id="01fee-103">tipo de recurso androidEnrollmentCompanyCode</span><span class="sxs-lookup"><span data-stu-id="01fee-103">androidEnrollmentCompanyCode resource type</span></span>

<span data-ttu-id="01fee-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01fee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="01fee-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="01fee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="01fee-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="01fee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="01fee-107">Uma classe para manter os dados de registro Specialty usados para registrar-se por meio da API de gerenciamento do Android do Google, como token, URL e conteúdo de código QR</span><span class="sxs-lookup"><span data-stu-id="01fee-107">A class to hold specialty enrollment data used for enrolling via Google's Android Management API, such as Token, Url, and QR code content</span></span>

## <a name="properties"></a><span data-ttu-id="01fee-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="01fee-108">Properties</span></span>
|<span data-ttu-id="01fee-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="01fee-109">Property</span></span>|<span data-ttu-id="01fee-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="01fee-110">Type</span></span>|<span data-ttu-id="01fee-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="01fee-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01fee-112">enrollmentToken</span><span class="sxs-lookup"><span data-stu-id="01fee-112">enrollmentToken</span></span>|<span data-ttu-id="01fee-113">String</span><span class="sxs-lookup"><span data-stu-id="01fee-113">String</span></span>|<span data-ttu-id="01fee-114">Token de registro usado pelo usuário para registrar seus dispositivos.</span><span class="sxs-lookup"><span data-stu-id="01fee-114">Enrollment Token used by the User to enroll their device.</span></span>|
|<span data-ttu-id="01fee-115">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="01fee-115">qrCodeContent</span></span>|<span data-ttu-id="01fee-116">String</span><span class="sxs-lookup"><span data-stu-id="01fee-116">String</span></span>|<span data-ttu-id="01fee-117">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="01fee-117">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="01fee-118">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="01fee-118">qrCodeImage</span></span>|[<span data-ttu-id="01fee-119">mimeContent</span><span class="sxs-lookup"><span data-stu-id="01fee-119">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="01fee-120">Código QR gerado para o token.</span><span class="sxs-lookup"><span data-stu-id="01fee-120">Generated QR code for the token.</span></span>|

## <a name="relationships"></a><span data-ttu-id="01fee-121">Relações</span><span class="sxs-lookup"><span data-stu-id="01fee-121">Relationships</span></span>
<span data-ttu-id="01fee-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="01fee-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="01fee-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="01fee-123">JSON Representation</span></span>
<span data-ttu-id="01fee-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="01fee-124">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidEnrollmentCompanyCode"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidEnrollmentCompanyCode",
  "enrollmentToken": "String",
  "qrCodeContent": "String",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "String",
    "value": "binary"
  }
}
```



