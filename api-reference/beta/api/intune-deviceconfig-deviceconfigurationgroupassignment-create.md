---
title: Criar deviceConfigurationGroupAssignment
description: Crie um novo objeto de deviceConfigurationGroupAssignment.
author: tfitzmac
ms.openlocfilehash: c07356d3cf63699fda95e2be6fe361841e0b0d95
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 12/18/2018
ms.locfileid: "27355101"
---
# <a name="create-deviceconfigurationgroupassignment"></a><span data-ttu-id="a7434-103">Criar deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="a7434-103">Create deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="a7434-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="a7434-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a7434-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="a7434-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a7434-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="a7434-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7434-107">Crie um novo objeto de [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="a7434-107">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a7434-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a7434-108">Prerequisites</span></span>
<span data-ttu-id="a7434-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a7434-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7434-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a7434-111">Permission type</span></span>|<span data-ttu-id="a7434-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="a7434-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7434-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a7434-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a7434-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7434-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a7434-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a7434-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7434-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7434-116">Not supported.</span></span>|
|<span data-ttu-id="a7434-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a7434-117">Application</span></span>|<span data-ttu-id="a7434-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a7434-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7434-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a7434-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="a7434-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a7434-120">Request headers</span></span>
|<span data-ttu-id="a7434-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a7434-121">Header</span></span>|<span data-ttu-id="a7434-122">Valor</span><span class="sxs-lookup"><span data-stu-id="a7434-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7434-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="a7434-123">Authorization</span></span>|<span data-ttu-id="a7434-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a7434-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7434-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a7434-125">Accept</span></span>|<span data-ttu-id="a7434-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a7434-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7434-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a7434-127">Request body</span></span>
<span data-ttu-id="a7434-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceConfigurationGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="a7434-128">In the request body, supply a JSON representation for the deviceConfigurationGroupAssignment object.</span></span>

<span data-ttu-id="a7434-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o deviceConfigurationGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="a7434-129">The following table shows the properties that are required when you create the deviceConfigurationGroupAssignment.</span></span>

|<span data-ttu-id="a7434-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a7434-130">Property</span></span>|<span data-ttu-id="a7434-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="a7434-131">Type</span></span>|<span data-ttu-id="a7434-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="a7434-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a7434-133">id</span><span class="sxs-lookup"><span data-stu-id="a7434-133">id</span></span>|<span data-ttu-id="a7434-134">String</span><span class="sxs-lookup"><span data-stu-id="a7434-134">String</span></span>|<span data-ttu-id="a7434-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a7434-135">Key of the entity.</span></span>|
|<span data-ttu-id="a7434-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="a7434-136">targetGroupId</span></span>|<span data-ttu-id="a7434-137">String</span><span class="sxs-lookup"><span data-stu-id="a7434-137">String</span></span>|<span data-ttu-id="a7434-138">A identificação do grupo AAD pretendemos a configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="a7434-138">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="a7434-139">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="a7434-139">excludeGroup</span></span>|<span data-ttu-id="a7434-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7434-140">Boolean</span></span>|<span data-ttu-id="a7434-141">Indica se este grupo devem ser excluídos.</span><span class="sxs-lookup"><span data-stu-id="a7434-141">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="a7434-142">Padrões que o grupo deve ser incluído</span><span class="sxs-lookup"><span data-stu-id="a7434-142">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="a7434-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7434-143">Response</span></span>
<span data-ttu-id="a7434-144">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a7434-144">If successful, this method returns a `201 Created` response code and a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7434-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a7434-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="a7434-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a7434-146">Request</span></span>
<span data-ttu-id="a7434-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a7434-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments
Content-type: application/json
Content-length: 146

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```

### <a name="response"></a><span data-ttu-id="a7434-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="a7434-148">Response</span></span>
<span data-ttu-id="a7434-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a7434-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 195

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```





