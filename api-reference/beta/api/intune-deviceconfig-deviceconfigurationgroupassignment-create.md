---
title: Criar deviceConfigurationGroupAssignment
description: Crie um novo objeto de deviceConfigurationGroupAssignment.
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f4193470483918a2b690962ae3e190a08ac2f4c0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/11/2019
ms.locfileid: "27869528"
---
# <a name="create-deviceconfigurationgroupassignment"></a><span data-ttu-id="ca324-103">Criar deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="ca324-103">Create deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="ca324-104">**Importante:** as APIs na versão /beta no Microsoft Graph estão em visualização e sujeitas a alterações.</span><span class="sxs-lookup"><span data-stu-id="ca324-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca324-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="ca324-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ca324-106">**Observação:** O uso das APIs do Microsoft Graph para configurar controles e políticas do Intune ainda exige que o serviço do Intune seja [corretamente licenciado](https://go.microsoft.com/fwlink/?linkid=839381) pelo cliente.</span><span class="sxs-lookup"><span data-stu-id="ca324-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ca324-107">Crie um novo objeto de [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="ca324-107">Create a new [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ca324-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="ca324-108">Prerequisites</span></span>
<span data-ttu-id="ca324-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="ca324-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca324-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="ca324-111">Permission type</span></span>|<span data-ttu-id="ca324-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="ca324-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca324-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="ca324-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca324-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca324-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ca324-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="ca324-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca324-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca324-116">Not supported.</span></span>|
|<span data-ttu-id="ca324-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="ca324-117">Application</span></span>|<span data-ttu-id="ca324-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="ca324-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca324-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="ca324-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="ca324-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="ca324-120">Request headers</span></span>
|<span data-ttu-id="ca324-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="ca324-121">Header</span></span>|<span data-ttu-id="ca324-122">Valor</span><span class="sxs-lookup"><span data-stu-id="ca324-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca324-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="ca324-123">Authorization</span></span>|<span data-ttu-id="ca324-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="ca324-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca324-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="ca324-125">Accept</span></span>|<span data-ttu-id="ca324-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca324-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca324-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="ca324-127">Request body</span></span>
<span data-ttu-id="ca324-128">No corpo da solicitação, fornece uma representação JSON para o objeto deviceConfigurationGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="ca324-128">In the request body, supply a JSON representation for the deviceConfigurationGroupAssignment object.</span></span>

<span data-ttu-id="ca324-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o deviceConfigurationGroupAssignment.</span><span class="sxs-lookup"><span data-stu-id="ca324-129">The following table shows the properties that are required when you create the deviceConfigurationGroupAssignment.</span></span>

|<span data-ttu-id="ca324-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="ca324-130">Property</span></span>|<span data-ttu-id="ca324-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="ca324-131">Type</span></span>|<span data-ttu-id="ca324-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="ca324-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca324-133">id</span><span class="sxs-lookup"><span data-stu-id="ca324-133">id</span></span>|<span data-ttu-id="ca324-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca324-134">String</span></span>|<span data-ttu-id="ca324-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="ca324-135">Key of the entity.</span></span>|
|<span data-ttu-id="ca324-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="ca324-136">targetGroupId</span></span>|<span data-ttu-id="ca324-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="ca324-137">String</span></span>|<span data-ttu-id="ca324-138">A identificação do grupo AAD pretendemos a configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="ca324-138">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="ca324-139">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="ca324-139">excludeGroup</span></span>|<span data-ttu-id="ca324-140">Booliano</span><span class="sxs-lookup"><span data-stu-id="ca324-140">Boolean</span></span>|<span data-ttu-id="ca324-141">Indica se este grupo devem ser excluídos.</span><span class="sxs-lookup"><span data-stu-id="ca324-141">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="ca324-142">Padrões que o grupo deve ser incluído</span><span class="sxs-lookup"><span data-stu-id="ca324-142">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="ca324-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca324-143">Response</span></span>
<span data-ttu-id="ca324-144">Se tiver êxito, este método retornará um `201 Created` código de resposta e um objeto [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="ca324-144">If successful, this method returns a `201 Created` response code and a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca324-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="ca324-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="ca324-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="ca324-146">Request</span></span>
<span data-ttu-id="ca324-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="ca324-147">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ca324-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="ca324-148">Response</span></span>
<span data-ttu-id="ca324-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="ca324-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





