---
title: Lista androidForWorkCertificateProfileBases
description: Lista as propriedades e os relacionamentos dos objetos androidForWorkCertificateProfileBase.
author: tfitzmac
ms.openlocfilehash: 2a0bd2de1408ad6fa41bb8b1e7be9d691460ceb9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318155"
---
# <a name="list-androidforworkcertificateprofilebases"></a><span data-ttu-id="034c9-103">Lista androidForWorkCertificateProfileBases</span><span class="sxs-lookup"><span data-stu-id="034c9-103">List androidForWorkCertificateProfileBases</span></span>

> <span data-ttu-id="034c9-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="034c9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="034c9-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="034c9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="034c9-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="034c9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="034c9-107">Lista as propriedades e os relacionamentos dos objetos [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md) .</span><span class="sxs-lookup"><span data-stu-id="034c9-107">List properties and relationships of the [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="034c9-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="034c9-108">Prerequisites</span></span>
<span data-ttu-id="034c9-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="034c9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="034c9-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="034c9-111">Permission type</span></span>|<span data-ttu-id="034c9-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="034c9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="034c9-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="034c9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="034c9-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="034c9-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="034c9-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="034c9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="034c9-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="034c9-116">Not supported.</span></span>|
|<span data-ttu-id="034c9-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="034c9-117">Application</span></span>|<span data-ttu-id="034c9-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="034c9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="034c9-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="034c9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="034c9-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="034c9-120">Request headers</span></span>
|<span data-ttu-id="034c9-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="034c9-121">Header</span></span>|<span data-ttu-id="034c9-122">Valor</span><span class="sxs-lookup"><span data-stu-id="034c9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="034c9-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="034c9-123">Authorization</span></span>|<span data-ttu-id="034c9-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="034c9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="034c9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="034c9-125">Accept</span></span>|<span data-ttu-id="034c9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="034c9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="034c9-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="034c9-127">Request body</span></span>
<span data-ttu-id="034c9-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="034c9-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="034c9-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="034c9-129">Response</span></span>
<span data-ttu-id="034c9-130">Se tiver êxito, este método retornará um `200 OK` código de resposta e uma coleção de objetos [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="034c9-130">If successful, this method returns a `200 OK` response code and a collection of [androidForWorkCertificateProfileBase](../resources/intune-deviceconfig-androidforworkcertificateprofilebase.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="034c9-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="034c9-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="034c9-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="034c9-132">Request</span></span>
<span data-ttu-id="034c9-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="034c9-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="034c9-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="034c9-134">Response</span></span>
<span data-ttu-id="034c9-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="034c9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 922

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidForWorkCertificateProfileBase",
      "id": "87f1d53b-d53b-87f1-3bd5-f1873bd5f187",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "renewalThresholdPercentage": 10,
      "subjectNameFormat": "commonNameIncludingEmail",
      "certificateValidityPeriodValue": 14,
      "certificateValidityPeriodScale": "months",
      "extendedKeyUsages": [
        {
          "@odata.type": "microsoft.graph.extendedKeyUsage",
          "name": "Name value",
          "objectIdentifier": "Object Identifier value"
        }
      ]
    }
  ]
}
```





