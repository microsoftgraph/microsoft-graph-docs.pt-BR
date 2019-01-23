---
title: tipo de recurso de androidEnrollmentCompanyCode
description: Uma classe para armazenar dados de registro de especialidade usados para inscrevendo por meio Android API do Google de gerenciamento, como Token, Url e QR conteúdo de código
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: be5b2a94445e95fe18271467b6661320d8204d76
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29428989"
---
# <a name="androidenrollmentcompanycode-resource-type"></a><span data-ttu-id="092fb-103">tipo de recurso de androidEnrollmentCompanyCode</span><span class="sxs-lookup"><span data-stu-id="092fb-103">androidEnrollmentCompanyCode resource type</span></span>

> <span data-ttu-id="092fb-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="092fb-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="092fb-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="092fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="092fb-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="092fb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="092fb-107">Uma classe para armazenar dados de registro de especialidade usados para inscrevendo por meio Android API do Google de gerenciamento, como Token, Url e QR conteúdo de código</span><span class="sxs-lookup"><span data-stu-id="092fb-107">A class to hold specialty enrollment data used for enrolling via Google's Android Management API, such as Token, Url, and QR code content</span></span>

## <a name="properties"></a><span data-ttu-id="092fb-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="092fb-108">Properties</span></span>
|<span data-ttu-id="092fb-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="092fb-109">Property</span></span>|<span data-ttu-id="092fb-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="092fb-110">Type</span></span>|<span data-ttu-id="092fb-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="092fb-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="092fb-112">enrollmentToken</span><span class="sxs-lookup"><span data-stu-id="092fb-112">enrollmentToken</span></span>|<span data-ttu-id="092fb-113">String</span><span class="sxs-lookup"><span data-stu-id="092fb-113">String</span></span>|<span data-ttu-id="092fb-114">Usado pelo usuário para registrar seus dispositivos de Token de inscrição.</span><span class="sxs-lookup"><span data-stu-id="092fb-114">Enrollment Token used by the User to enroll their device.</span></span>|
|<span data-ttu-id="092fb-115">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="092fb-115">qrCodeContent</span></span>|<span data-ttu-id="092fb-116">String</span><span class="sxs-lookup"><span data-stu-id="092fb-116">String</span></span>|<span data-ttu-id="092fb-117">Cadeia de caracteres usada para gerar um código QR para o token.</span><span class="sxs-lookup"><span data-stu-id="092fb-117">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="092fb-118">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="092fb-118">qrCodeImage</span></span>|[<span data-ttu-id="092fb-119">mimeContent</span><span class="sxs-lookup"><span data-stu-id="092fb-119">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="092fb-120">Código QR gerado para o token.</span><span class="sxs-lookup"><span data-stu-id="092fb-120">Generated QR code for the token.</span></span>|

## <a name="relationships"></a><span data-ttu-id="092fb-121">Relações</span><span class="sxs-lookup"><span data-stu-id="092fb-121">Relationships</span></span>
<span data-ttu-id="092fb-122">Nenhum</span><span class="sxs-lookup"><span data-stu-id="092fb-122">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="092fb-123">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="092fb-123">JSON Representation</span></span>
<span data-ttu-id="092fb-124">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="092fb-124">Here is a JSON representation of the resource.</span></span>
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




