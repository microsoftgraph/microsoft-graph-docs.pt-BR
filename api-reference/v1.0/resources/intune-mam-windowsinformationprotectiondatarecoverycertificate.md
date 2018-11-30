---
title: Tipo de recurso windowsInformationProtectionDataRecoveryCertificate
description: DataRecoveryCertificate da proteção de informações do Windows
ms.openlocfilehash: 68faf0e78c68468216c3e69d64926f2c8b18e3c4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27006045"
---
# <a name="windowsinformationprotectiondatarecoverycertificate-resource-type"></a><span data-ttu-id="a0e83-103">Tipo de recurso windowsInformationProtectionDataRecoveryCertificate</span><span class="sxs-lookup"><span data-stu-id="a0e83-103">windowsInformationProtectionDataRecoveryCertificate resource type</span></span>

> <span data-ttu-id="a0e83-104">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a0e83-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a0e83-105">DataRecoveryCertificate da proteção de informações do Windows</span><span class="sxs-lookup"><span data-stu-id="a0e83-105">Windows Information Protection DataRecoveryCertificate</span></span>
## <a name="properties"></a><span data-ttu-id="a0e83-106">Propriedades</span><span class="sxs-lookup"><span data-stu-id="a0e83-106">Properties</span></span>
|<span data-ttu-id="a0e83-107">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a0e83-107">Property</span></span>|<span data-ttu-id="a0e83-108">Tipo</span><span class="sxs-lookup"><span data-stu-id="a0e83-108">Type</span></span>|<span data-ttu-id="a0e83-109">Descrição</span><span class="sxs-lookup"><span data-stu-id="a0e83-109">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a0e83-110">SubjectName</span><span class="sxs-lookup"><span data-stu-id="a0e83-110">subjectName</span></span>|<span data-ttu-id="a0e83-111">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0e83-111">String</span></span>|<span data-ttu-id="a0e83-112">Nome do assunto do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="a0e83-112">Data recovery Certificate subject name</span></span>|
|<span data-ttu-id="a0e83-113">descrição</span><span class="sxs-lookup"><span data-stu-id="a0e83-113">description</span></span>|<span data-ttu-id="a0e83-114">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="a0e83-114">String</span></span>|<span data-ttu-id="a0e83-115">Descrição do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="a0e83-115">Data recovery Certificate description</span></span>|
|<span data-ttu-id="a0e83-116">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="a0e83-116">expirationDateTime</span></span>|<span data-ttu-id="a0e83-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a0e83-117">DateTimeOffset</span></span>|<span data-ttu-id="a0e83-118">Datetime de vencimento do certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="a0e83-118">Data recovery Certificate expiration datetime</span></span>|
|<span data-ttu-id="a0e83-119">certificado</span><span class="sxs-lookup"><span data-stu-id="a0e83-119">certificate</span></span>|<span data-ttu-id="a0e83-120">Binário</span><span class="sxs-lookup"><span data-stu-id="a0e83-120">Binary</span></span>|<span data-ttu-id="a0e83-121">Certificado de recuperação de dados</span><span class="sxs-lookup"><span data-stu-id="a0e83-121">Data recovery Certificate</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0e83-122">Relações</span><span class="sxs-lookup"><span data-stu-id="a0e83-122">Relationships</span></span>
<span data-ttu-id="a0e83-123">Nenhum</span><span class="sxs-lookup"><span data-stu-id="a0e83-123">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a0e83-124">Representação JSON</span><span class="sxs-lookup"><span data-stu-id="a0e83-124">JSON Representation</span></span>
<span data-ttu-id="a0e83-125">Veja a seguir uma representação JSON do recurso.</span><span class="sxs-lookup"><span data-stu-id="a0e83-125">Here is a JSON representation of the resource.</span></span>
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



