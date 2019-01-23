---
title: Excluir deviceConfigurationGroupAssignment
description: Exclui um deviceConfigurationGroupAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 7f63a2443982ba86be637b4da45314bb6ad9fcd9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29398083"
---
# <a name="delete-deviceconfigurationgroupassignment"></a><span data-ttu-id="60bf3-103">Excluir deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="60bf3-103">Delete deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="60bf3-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="60bf3-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="60bf3-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="60bf3-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="60bf3-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="60bf3-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60bf3-107">Exclui um [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="60bf3-107">Deletes a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60bf3-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="60bf3-108">Prerequisites</span></span>
<span data-ttu-id="60bf3-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="60bf3-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="60bf3-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="60bf3-111">Permission type</span></span>|<span data-ttu-id="60bf3-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="60bf3-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60bf3-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="60bf3-113">Delegated (work or school account)</span></span>|<span data-ttu-id="60bf3-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60bf3-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="60bf3-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="60bf3-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60bf3-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60bf3-116">Not supported.</span></span>|
|<span data-ttu-id="60bf3-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="60bf3-117">Application</span></span>|<span data-ttu-id="60bf3-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="60bf3-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60bf3-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="60bf3-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments/{deviceConfigurationGroupAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="60bf3-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="60bf3-120">Request headers</span></span>
|<span data-ttu-id="60bf3-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="60bf3-121">Header</span></span>|<span data-ttu-id="60bf3-122">Valor</span><span class="sxs-lookup"><span data-stu-id="60bf3-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60bf3-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="60bf3-123">Authorization</span></span>|<span data-ttu-id="60bf3-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="60bf3-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60bf3-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="60bf3-125">Accept</span></span>|<span data-ttu-id="60bf3-126">application/json</span><span class="sxs-lookup"><span data-stu-id="60bf3-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60bf3-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="60bf3-127">Request body</span></span>
<span data-ttu-id="60bf3-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="60bf3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60bf3-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="60bf3-129">Response</span></span>
<span data-ttu-id="60bf3-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="60bf3-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="60bf3-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="60bf3-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="60bf3-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="60bf3-132">Request</span></span>
<span data-ttu-id="60bf3-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="60bf3-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

### <a name="response"></a><span data-ttu-id="60bf3-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="60bf3-134">Response</span></span>
<span data-ttu-id="60bf3-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="60bf3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




