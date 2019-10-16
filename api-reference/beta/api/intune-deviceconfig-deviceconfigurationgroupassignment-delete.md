---
title: Excluir deviceConfigurationGroupAssignment
description: Exclui deviceConfigurationGroupAssignment.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c32b44ddcbb9e0cc44df1121d530097ea2e8a398
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 10/16/2019
ms.locfileid: "37534068"
---
# <a name="delete-deviceconfigurationgroupassignment"></a><span data-ttu-id="b9cbc-103">Excluir deviceConfigurationGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="b9cbc-103">Delete deviceConfigurationGroupAssignment</span></span>

> <span data-ttu-id="b9cbc-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="b9cbc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9cbc-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="b9cbc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9cbc-106">Exclui [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span><span class="sxs-lookup"><span data-stu-id="b9cbc-106">Deletes a [deviceConfigurationGroupAssignment](../resources/intune-deviceconfig-deviceconfigurationgroupassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9cbc-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="b9cbc-107">Prerequisites</span></span>
<span data-ttu-id="b9cbc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b9cbc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9cbc-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="b9cbc-110">Permission type</span></span>|<span data-ttu-id="b9cbc-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="b9cbc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9cbc-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="b9cbc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b9cbc-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9cbc-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b9cbc-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="b9cbc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9cbc-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="b9cbc-115">Not supported.</span></span>|
|<span data-ttu-id="b9cbc-116">Application</span><span class="sxs-lookup"><span data-stu-id="b9cbc-116">Application</span></span>|<span data-ttu-id="b9cbc-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9cbc-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9cbc-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="b9cbc-118">HTTP Request</span></span>
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
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/groupAssignments/{deviceConfigurationGroupAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/groupAssignments/{deviceConfigurationGroupAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b9cbc-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="b9cbc-119">Request headers</span></span>
|<span data-ttu-id="b9cbc-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="b9cbc-120">Header</span></span>|<span data-ttu-id="b9cbc-121">Valor</span><span class="sxs-lookup"><span data-stu-id="b9cbc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9cbc-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="b9cbc-122">Authorization</span></span>|<span data-ttu-id="b9cbc-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="b9cbc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9cbc-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="b9cbc-124">Accept</span></span>|<span data-ttu-id="b9cbc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b9cbc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9cbc-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="b9cbc-126">Request body</span></span>
<span data-ttu-id="b9cbc-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="b9cbc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9cbc-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9cbc-128">Response</span></span>
<span data-ttu-id="b9cbc-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="b9cbc-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b9cbc-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="b9cbc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9cbc-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="b9cbc-131">Request</span></span>
<span data-ttu-id="b9cbc-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="b9cbc-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}
```

### <a name="response"></a><span data-ttu-id="b9cbc-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="b9cbc-133">Response</span></span>
<span data-ttu-id="b9cbc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="b9cbc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






