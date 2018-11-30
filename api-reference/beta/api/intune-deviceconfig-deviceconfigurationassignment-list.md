---
title: Listar deviceConfigurationAssignments
description: Listar propriedades e relações dos objetos deviceConfigurationAssignment.
ms.openlocfilehash: 51d4ea7c0c5a49b59777d5deaa364a8791a7db8f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/29/2018
ms.locfileid: "27034206"
---
# <a name="list-deviceconfigurationassignments"></a><span data-ttu-id="b6a5a-103">Listar deviceConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="b6a5a-103">List deviceConfigurationAssignments</span></span>

> <span data-ttu-id="b6a5a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="b6a5a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6a5a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="b6a5a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6a5a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="b6a5a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6a5a-107">Listar propriedades e relações dos objetos [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b6a5a-107">List properties and relationships of the [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b6a5a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b6a5a-108">Prerequisites</span></span>
<span data-ttu-id="b6a5a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b6a5a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6a5a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b6a5a-111">Permission type</span></span>|<span data-ttu-id="b6a5a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b6a5a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6a5a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b6a5a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6a5a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6a5a-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b6a5a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b6a5a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6a5a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6a5a-116">Not supported.</span></span>|
|<span data-ttu-id="b6a5a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="b6a5a-117">Application</span></span>|<span data-ttu-id="b6a5a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b6a5a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6a5a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b6a5a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="b6a5a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b6a5a-120">Request headers</span></span>
|<span data-ttu-id="b6a5a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b6a5a-121">Header</span></span>|<span data-ttu-id="b6a5a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="b6a5a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6a5a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="b6a5a-123">Authorization</span></span>|<span data-ttu-id="b6a5a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b6a5a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6a5a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b6a5a-125">Accept</span></span>|<span data-ttu-id="b6a5a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6a5a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6a5a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b6a5a-127">Request body</span></span>
<span data-ttu-id="b6a5a-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b6a5a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6a5a-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6a5a-129">Response</span></span>
<span data-ttu-id="b6a5a-130">Se tiver êxito, este método retornará um código de resposta `200 OK` e uma coleção de objetos [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="b6a5a-130">If successful, this method returns a `200 OK` response code and a collection of [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6a5a-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b6a5a-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="b6a5a-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b6a5a-132">Request</span></span>
<span data-ttu-id="b6a5a-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b6a5a-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="b6a5a-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="b6a5a-134">Response</span></span>
<span data-ttu-id="b6a5a-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b6a5a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 271

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
      "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





