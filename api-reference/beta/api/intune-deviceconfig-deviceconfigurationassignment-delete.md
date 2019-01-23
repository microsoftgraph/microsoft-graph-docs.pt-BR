---
title: Excluir deviceConfigurationAssignment
description: Exclui deviceConfigurationAssignment.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e148f00d6c568e42a6b2ee8a77059605efecb1bf
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29415961"
---
# <a name="delete-deviceconfigurationassignment"></a><span data-ttu-id="e1279-103">Excluir deviceConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="e1279-103">Delete deviceConfigurationAssignment</span></span>

> <span data-ttu-id="e1279-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="e1279-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e1279-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="e1279-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e1279-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="e1279-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e1279-107">Exclui [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span><span class="sxs-lookup"><span data-stu-id="e1279-107">Deletes a [deviceConfigurationAssignment](../resources/intune-deviceconfig-deviceconfigurationassignment.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e1279-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e1279-108">Prerequisites</span></span>
<span data-ttu-id="e1279-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="e1279-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e1279-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e1279-111">Permission type</span></span>|<span data-ttu-id="e1279-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e1279-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e1279-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e1279-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e1279-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e1279-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e1279-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e1279-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e1279-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1279-116">Not supported.</span></span>|
|<span data-ttu-id="e1279-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e1279-117">Application</span></span>|<span data-ttu-id="e1279-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e1279-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e1279-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e1279-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/identityCertificate/rootCertificate/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.iosScepCertificateProfile/rootCertificate/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.macOSScepCertificateProfile/rootCertificate/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/identityCertificateForClientAuthentication/assignments/{deviceConfigurationAssignmentId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsWifiEnterpriseEAPConfiguration/rootCertificatesForServerValidation/{windows81TrustedRootCertificateId}/assignments/{deviceConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="e1279-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e1279-120">Request headers</span></span>
|<span data-ttu-id="e1279-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e1279-121">Header</span></span>|<span data-ttu-id="e1279-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e1279-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e1279-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e1279-123">Authorization</span></span>|<span data-ttu-id="e1279-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e1279-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e1279-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e1279-125">Accept</span></span>|<span data-ttu-id="e1279-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e1279-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e1279-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e1279-127">Request body</span></span>
<span data-ttu-id="e1279-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e1279-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e1279-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1279-129">Response</span></span>
<span data-ttu-id="e1279-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e1279-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e1279-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e1279-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e1279-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e1279-132">Request</span></span>
<span data-ttu-id="e1279-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e1279-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/assignments/{deviceConfigurationAssignmentId}
```

### <a name="response"></a><span data-ttu-id="e1279-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e1279-134">Response</span></span>
<span data-ttu-id="e1279-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e1279-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




