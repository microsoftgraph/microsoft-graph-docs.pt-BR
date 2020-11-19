---
title: Excluir deviceEnrollmentWindowsHelloForBusinessConfiguration
description: Exclui deviceEnrollmentWindowsHelloForBusinessConfiguration.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0608e8de8064b4176c3bfd64e80583c7b5416e31
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 11/18/2020
ms.locfileid: "49262200"
---
# <a name="delete-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="d87f2-103">Excluir deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="d87f2-103">Delete deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

<span data-ttu-id="d87f2-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d87f2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d87f2-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="d87f2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d87f2-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="d87f2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d87f2-107">Exclui [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span><span class="sxs-lookup"><span data-stu-id="d87f2-107">Deletes a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d87f2-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="d87f2-108">Prerequisites</span></span>
<span data-ttu-id="d87f2-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="d87f2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d87f2-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="d87f2-111">Permission type</span></span>|<span data-ttu-id="d87f2-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="d87f2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d87f2-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="d87f2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d87f2-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d87f2-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="d87f2-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="d87f2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d87f2-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="d87f2-116">Not supported.</span></span>|
|<span data-ttu-id="d87f2-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="d87f2-117">Application</span></span>|<span data-ttu-id="d87f2-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d87f2-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d87f2-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="d87f2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d87f2-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="d87f2-120">Request headers</span></span>
|<span data-ttu-id="d87f2-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="d87f2-121">Header</span></span>|<span data-ttu-id="d87f2-122">Valor</span><span class="sxs-lookup"><span data-stu-id="d87f2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d87f2-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="d87f2-123">Authorization</span></span>|<span data-ttu-id="d87f2-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="d87f2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d87f2-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="d87f2-125">Accept</span></span>|<span data-ttu-id="d87f2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d87f2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d87f2-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="d87f2-127">Request body</span></span>
<span data-ttu-id="d87f2-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="d87f2-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d87f2-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="d87f2-129">Response</span></span>
<span data-ttu-id="d87f2-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="d87f2-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d87f2-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="d87f2-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d87f2-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="d87f2-132">Request</span></span>
<span data-ttu-id="d87f2-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="d87f2-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d87f2-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="d87f2-134">Response</span></span>
<span data-ttu-id="d87f2-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="d87f2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




