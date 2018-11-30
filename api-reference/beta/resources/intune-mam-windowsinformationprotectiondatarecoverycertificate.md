---
title: Tipo de recurso windowsInformationProtectionDataRecoveryCertificate
description: DataRecoveryCertificate da proteção de informações do Windows
ms.openlocfilehash: bbc6ae8e4607e5992ac9dd23fa1eb67e51d1ecd4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034789"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="2b2ca-103">Tipo de recurso windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="2b2ca-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="2b2ca-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e estão sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="2b2ca-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b2ca-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="2b2ca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2b2ca-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="2b2ca-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2b2ca-107">DataRecoveryCertificate da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="2b2ca-107">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="2b2ca-108">Propriedades</span><span class="sxs-lookup"><span data-stu-id="2b2ca-108">Properties</span></span>
|<span data-ttu-id="2b2ca-109">Propriedade</span><span class="sxs-lookup"><span data-stu-id="2b2ca-109">Property</span></span>|<span data-ttu-id="2b2ca-110">Tipo</span><span class="sxs-lookup"><span data-stu-id="2b2ca-110">Type</span></span>|<span data-ttu-id="2b2ca-111">Descrição</span><span class="sxs-lookup"><span data-stu-id="2b2ca-111">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b2ca-112">SubjectName</span><span class="sxs-lookup"><span data-stu-id="2b2ca-112">subjectName</span></span>|<span data-ttu-id="2b2ca-113">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2b2ca-113">String</span></span>|<span data-ttu-id="2b2ca-114">Nome do assunto do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="2b2ca-114">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="2b2ca-115">descrição</span><span class="sxs-lookup"><span data-stu-id="2b2ca-115">description</span></span>|<span data-ttu-id="2b2ca-116">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="2b2ca-116">String</span></span>|<span data-ttu-id="2b2ca-117">Descrição do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="2b2ca-117">Data recovery Certificate description</span></span>|
|<span data-ttu-id="2b2ca-118">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2b2ca-118">expirationDateTime</span></span>|<span data-ttu-id="2b2ca-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2b2ca-119">DateTimeOffset</span></span>|<span data-ttu-id="2b2ca-120">Datetime de vencimento do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="2b2ca-120">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="2b2ca-121">certificado</span><span class="sxs-lookup"><span data-stu-id="2b2ca-121">certificate</span></span>|<span data-ttu-id="2b2ca-122">Binário</span><span class="sxs-lookup"><span data-stu-id="2b2ca-122">Binary</span></span>|<span data-ttu-id="2b2ca-123">Certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="2b2ca-123">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="2b2ca-124">Relações</span><span class="sxs-lookup"><span data-stu-id="2b2ca-124">Relationships</span></span>
<span data-ttu-id="2b2ca-125">Nenhum</span><span class="sxs-lookup"><span data-stu-id="2b2ca-125">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2b2ca-126">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="2b2ca-126">JSON Representation</span></span>
<span data-ttu-id="2b2ca-127">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="2b2ca-127">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsInformationProtectionDataRecoveryCertificate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionDataRecoveryCertificate",
  "subjectName": "String",
  "description": "String",
  "expirationDateTime": "String (timestamp)",
  "certificate": "binary"
}
```





