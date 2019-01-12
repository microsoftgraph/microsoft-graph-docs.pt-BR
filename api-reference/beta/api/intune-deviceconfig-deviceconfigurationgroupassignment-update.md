---
title: Atualizar deviceConfigurationGroupAssignment
description: Atualize as propriedades de um objeto deviceConfigurationGroupAssignment.
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 632ade6d8c2fdb2cfb859c3b480606547d9b0ead
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/12/2019
ms.locfileid: "27938514"
---
# <a name="update-deviceconfigurationgroupassignment"></a><span data-ttu-id="e5c4a-103">Atualizar deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="e5c4a-103">Update deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="e5c4a-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="e5c4a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e5c4a-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e5c4a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e5c4a-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="e5c4a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e5c4a-107">Atualize as propriedades de um objeto [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e5c4a-107">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e5c4a-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e5c4a-108">Prerequisites</span></span>
<span data-ttu-id="e5c4a-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e5c4a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e5c4a-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e5c4a-111">Permission type</span></span>|<span data-ttu-id="e5c4a-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e5c4a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e5c4a-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e5c4a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e5c4a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e5c4a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e5c4a-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e5c4a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e5c4a-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5c4a-116">Not supported.</span></span>|
|<span data-ttu-id="e5c4a-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e5c4a-117">Application</span></span>|<span data-ttu-id="e5c4a-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e5c4a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e5c4a-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e5c4a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments/{deviceConfigurationGroupAssignmentId}
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="e5c4a-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e5c4a-120">Request headers</span></span>
|<span data-ttu-id="e5c4a-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e5c4a-121">Header</span></span>|<span data-ttu-id="e5c4a-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e5c4a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e5c4a-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e5c4a-123">Authorization</span></span>|<span data-ttu-id="e5c4a-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e5c4a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e5c4a-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e5c4a-125">Accept</span></span>|<span data-ttu-id="e5c4a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e5c4a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e5c4a-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e5c4a-127">Request body</span></span>
<span data-ttu-id="e5c4a-128">No corpo da solicitação, fornece uma representação JSON para o objeto [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="e5c4a-128">In the request body, supply a JSON representation for the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

<span data-ttu-id="e5c4a-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e5c4a-129">The following table shows the properties that are required when you create the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>

|<span data-ttu-id="e5c4a-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="e5c4a-130">Property</span></span>|<span data-ttu-id="e5c4a-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="e5c4a-131">Type</span></span>|<span data-ttu-id="e5c4a-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="e5c4a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5c4a-133">id</span><span class="sxs-lookup"><span data-stu-id="e5c4a-133">id</span></span>|<span data-ttu-id="e5c4a-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5c4a-134">String</span></span>|<span data-ttu-id="e5c4a-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="e5c4a-135">Key of the entity.</span></span>|
|<span data-ttu-id="e5c4a-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="e5c4a-136">targetGroupId</span></span>|<span data-ttu-id="e5c4a-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="e5c4a-137">String</span></span>|<span data-ttu-id="e5c4a-138">A identificação do grupo AAD pretendemos a configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="e5c4a-138">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="e5c4a-139">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="e5c4a-139">excludeGroup</span></span>|<span data-ttu-id="e5c4a-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="e5c4a-140">Boolean</span></span>|<span data-ttu-id="e5c4a-141">Indica se este grupo devem ser excluídos.</span><span class="sxs-lookup"><span data-stu-id="e5c4a-141">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="e5c4a-142">Padrões que o grupo deve ser incluído</span><span class="sxs-lookup"><span data-stu-id="e5c4a-142">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="e5c4a-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5c4a-143">Response</span></span>
<span data-ttu-id="e5c4a-144">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="e5c4a-144">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e5c4a-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e5c4a-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="e5c4a-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e5c4a-146">Request</span></span>
<span data-ttu-id="e5c4a-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e5c4a-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
Content-type: application/json
Content-length: 73

{
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```

### <a name="response"></a><span data-ttu-id="e5c4a-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="e5c4a-148">Response</span></span>
<span data-ttu-id="e5c4a-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e5c4a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 195

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "id": "561d26c5-26c5-561d-c526-1d56c5261d56",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```





