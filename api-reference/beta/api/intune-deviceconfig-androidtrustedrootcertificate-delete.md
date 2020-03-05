---
title: Excluir androidTrustedRootCertificate
description: Exclui androidTrustedRootCertificate.
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6dfef6b1d8d405ff8ded49fa06da4e1b3063d711
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/05/2020
ms.locfileid: "42443633"
---
# <a name="delete-androidtrustedrootcertificate"></a><span data-ttu-id="e8cdc-103">Excluir androidTrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="e8cdc-103">Delete androidTrustedRootCertificate</span></span>

<span data-ttu-id="e8cdc-104">Namespace: Microsoft. Graph</span><span class="sxs-lookup"><span data-stu-id="e8cdc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e8cdc-105">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="e8cdc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8cdc-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="e8cdc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8cdc-107">Exclui [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="e8cdc-107">Deletes a [androidTrustedRootCertificate](../resources/intune-deviceconfig-androidtrustedrootcertificate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8cdc-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="e8cdc-108">Prerequisites</span></span>
<span data-ttu-id="e8cdc-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e8cdc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8cdc-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="e8cdc-111">Permission type</span></span>|<span data-ttu-id="e8cdc-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="e8cdc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8cdc-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="e8cdc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e8cdc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8cdc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e8cdc-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="e8cdc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8cdc-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="e8cdc-116">Not supported.</span></span>|
|<span data-ttu-id="e8cdc-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="e8cdc-117">Application</span></span>|<span data-ttu-id="e8cdc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8cdc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8cdc-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="e8cdc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidCertificateProfileBase/rootCertificate
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.androidEnterpriseWiFiConfiguration/rootCertificateForServerValidation
```

## <a name="request-headers"></a><span data-ttu-id="e8cdc-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="e8cdc-120">Request headers</span></span>
|<span data-ttu-id="e8cdc-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="e8cdc-121">Header</span></span>|<span data-ttu-id="e8cdc-122">Valor</span><span class="sxs-lookup"><span data-stu-id="e8cdc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8cdc-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="e8cdc-123">Authorization</span></span>|<span data-ttu-id="e8cdc-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="e8cdc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8cdc-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="e8cdc-125">Accept</span></span>|<span data-ttu-id="e8cdc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e8cdc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8cdc-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="e8cdc-127">Request body</span></span>
<span data-ttu-id="e8cdc-128">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="e8cdc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e8cdc-129">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8cdc-129">Response</span></span>
<span data-ttu-id="e8cdc-130">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="e8cdc-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e8cdc-131">Exemplo</span><span class="sxs-lookup"><span data-stu-id="e8cdc-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8cdc-132">Solicitação</span><span class="sxs-lookup"><span data-stu-id="e8cdc-132">Request</span></span>
<span data-ttu-id="e8cdc-133">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="e8cdc-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/rootCertificate
```

### <a name="response"></a><span data-ttu-id="e8cdc-134">Resposta</span><span class="sxs-lookup"><span data-stu-id="e8cdc-134">Response</span></span>
<span data-ttu-id="e8cdc-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="e8cdc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





