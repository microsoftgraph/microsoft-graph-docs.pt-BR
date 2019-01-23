---
title: Atualizar deviceConfigurationGroupAssignment
description: Atualize as propriedades de um objeto deviceConfigurationGroupAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 93399328a5be63bcb994fab58b6cad638a44d97f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29396282"
---
# <a name="update-deviceconfigurationgroupassignment"></a><span data-ttu-id="4c0d4-103">Atualizar deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="4c0d4-103">Update deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="4c0d4-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="4c0d4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4c0d4-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="4c0d4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4c0d4-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="4c0d4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c0d4-107">Atualize as propriedades de um objeto [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="4c0d4-107">Update the properties of a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c0d4-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4c0d4-108">Prerequisites</span></span>
<span data-ttu-id="4c0d4-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4c0d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4c0d4-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4c0d4-111">Permission type</span></span>|<span data-ttu-id="4c0d4-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4c0d4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c0d4-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4c0d4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4c0d4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c0d4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4c0d4-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4c0d4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c0d4-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c0d4-116">Not supported.</span></span>|
|<span data-ttu-id="4c0d4-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4c0d4-117">Application</span></span>|<span data-ttu-id="4c0d4-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4c0d4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c0d4-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4c0d4-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="4c0d4-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4c0d4-120">Request headers</span></span>
|<span data-ttu-id="4c0d4-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4c0d4-121">Header</span></span>|<span data-ttu-id="4c0d4-122">Valor</span><span class="sxs-lookup"><span data-stu-id="4c0d4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c0d4-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="4c0d4-123">Authorization</span></span>|<span data-ttu-id="4c0d4-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4c0d4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c0d4-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4c0d4-125">Accept</span></span>|<span data-ttu-id="4c0d4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4c0d4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c0d4-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4c0d4-127">Request body</span></span>
<span data-ttu-id="4c0d4-128">No corpo da solicitação, fornece uma representação JSON para o objeto [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) .</span><span class="sxs-lookup"><span data-stu-id="4c0d4-128">In the request body, supply a JSON representation for the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object.</span></span>

<span data-ttu-id="4c0d4-129">A tabela a seguir mostra as propriedades que são necessárias quando você cria o [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="4c0d4-129">The following table shows the properties that are required when you create the [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>

|<span data-ttu-id="4c0d4-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4c0d4-130">Property</span></span>|<span data-ttu-id="4c0d4-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="4c0d4-131">Type</span></span>|<span data-ttu-id="4c0d4-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="4c0d4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c0d4-133">id</span><span class="sxs-lookup"><span data-stu-id="4c0d4-133">id</span></span>|<span data-ttu-id="4c0d4-134">String</span><span class="sxs-lookup"><span data-stu-id="4c0d4-134">String</span></span>|<span data-ttu-id="4c0d4-135">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="4c0d4-135">Key of the entity.</span></span>|
|<span data-ttu-id="4c0d4-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="4c0d4-136">targetGroupId</span></span>|<span data-ttu-id="4c0d4-137">String</span><span class="sxs-lookup"><span data-stu-id="4c0d4-137">String</span></span>|<span data-ttu-id="4c0d4-138">A identificação do grupo AAD pretendemos a configuração do dispositivo.</span><span class="sxs-lookup"><span data-stu-id="4c0d4-138">The Id of the AAD group we are targeting the device configuration to.</span></span>|
|<span data-ttu-id="4c0d4-139">excludeGroup</span><span class="sxs-lookup"><span data-stu-id="4c0d4-139">excludeGroup</span></span>|<span data-ttu-id="4c0d4-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c0d4-140">Boolean</span></span>|<span data-ttu-id="4c0d4-141">Indica se este grupo devem ser excluídos.</span><span class="sxs-lookup"><span data-stu-id="4c0d4-141">Indicates if this group is should be excluded.</span></span> <span data-ttu-id="4c0d4-142">Padrões que o grupo deve ser incluído</span><span class="sxs-lookup"><span data-stu-id="4c0d4-142">Defaults that the group should be included</span></span>|



## <a name="response"></a><span data-ttu-id="4c0d4-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c0d4-143">Response</span></span>
<span data-ttu-id="4c0d4-144">Se tiver êxito, este método retornará um `200 OK` código de resposta e um objeto atualizado [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4c0d4-144">If successful, this method returns a `200 OK` response code and an updated [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c0d4-145">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4c0d4-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c0d4-146">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4c0d4-146">Request</span></span>
<span data-ttu-id="4c0d4-147">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4c0d4-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
Content-type: application/json
Content-length: 146

{
  "@odata.type": "#microsoft.graph.deviceConfigurationGroupAssignment",
  "targetGroupId": "Target Group Id value",
  "excludeGroup": true
}
```

### <a name="response"></a><span data-ttu-id="4c0d4-148">Resposta</span><span class="sxs-lookup"><span data-stu-id="4c0d4-148">Response</span></span>
<span data-ttu-id="4c0d4-p104">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4c0d4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




