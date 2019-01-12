---
title: Criar deviceConfigurationAssignment
description: Criar um novo objeto deviceConfigurationAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e555254f473b119b5a1e27cb2c5823e7863060fc
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27979170"
---
# <a name="create-deviceconfigurationassignment"></a><span data-ttu-id="6ea1e-103">Criar deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6ea1e-103">Create deviceConfigurationAssignment</span></span>

> <span data-ttu-id="6ea1e-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ea1e-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6ea1e-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6ea1e-107">Criar um novo objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="6ea1e-107">Create a new [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6ea1e-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="6ea1e-108">Prerequisites</span></span>
<span data-ttu-id="6ea1e-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6ea1e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ea1e-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="6ea1e-111">Permission type</span></span>|<span data-ttu-id="6ea1e-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="6ea1e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ea1e-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="6ea1e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6ea1e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6ea1e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6ea1e-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="6ea1e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ea1e-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-116">Not supported.</span></span>|
|<span data-ttu-id="6ea1e-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="6ea1e-117">Application</span></span>|<span data-ttu-id="6ea1e-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ea1e-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="6ea1e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="6ea1e-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="6ea1e-120">Request headers</span></span>
|<span data-ttu-id="6ea1e-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="6ea1e-121">Header</span></span>|<span data-ttu-id="6ea1e-122">Valor</span><span class="sxs-lookup"><span data-stu-id="6ea1e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ea1e-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="6ea1e-123">Authorization</span></span>|<span data-ttu-id="6ea1e-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ea1e-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="6ea1e-125">Accept</span></span>|<span data-ttu-id="6ea1e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6ea1e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ea1e-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="6ea1e-127">Request body</span></span>
<span data-ttu-id="6ea1e-128">No corpo da solicitação, forneça uma representação JSON do objeto deviceConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-128">In the request body, supply a JSON representation for the deviceConfigurationAssignment object.</span></span>

<span data-ttu-id="6ea1e-129">A tabela a seguir mostra as propriedades que são necessárias ao criar deviceConfigurationAssignment.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-129">The following table shows the properties that are required when you create the deviceConfigurationAssignment.</span></span>

|<span data-ttu-id="6ea1e-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="6ea1e-130">Property</span></span>|<span data-ttu-id="6ea1e-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="6ea1e-131">Type</span></span>|<span data-ttu-id="6ea1e-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="6ea1e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ea1e-133">id</span><span class="sxs-lookup"><span data-stu-id="6ea1e-133">id</span></span>|<span data-ttu-id="6ea1e-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="6ea1e-134">String</span></span>|<span data-ttu-id="6ea1e-135">A chave da atribuição.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-135">The key of the assignment.</span></span>|
|<span data-ttu-id="6ea1e-136">destino</span><span class="sxs-lookup"><span data-stu-id="6ea1e-136">target</span></span>|[<span data-ttu-id="6ea1e-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6ea1e-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="6ea1e-138">O destino da atribuição da configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-138">The assignment target for the device configuration.</span></span>|



## <a name="response"></a><span data-ttu-id="6ea1e-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ea1e-139">Response</span></span>
<span data-ttu-id="6ea1e-140">Se tiver êxito, este método retornará um código de resposta `201 Created` e um objeto [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-140">If successful, this method returns a `201 Created` response code and a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ea1e-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="6ea1e-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="6ea1e-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="6ea1e-142">Request</span></span>
<span data-ttu-id="6ea1e-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments
Content-type: application/json
Content-length: 169

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="6ea1e-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="6ea1e-144">Response</span></span>
<span data-ttu-id="6ea1e-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="6ea1e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 218

{
  "@odata.type": "#microsoft.graph.deviceConfigurationAssignment",
  "id": "d59b6342-6342-d59b-4263-9bd542639bd5",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





