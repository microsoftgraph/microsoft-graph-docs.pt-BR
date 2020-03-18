---
title: Excluir windowsPhone81TrustedRootCertificate
description: Exclui windowsPhone81TrustedRootCertificate.
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a3bd7854e56bf9041cc63493c7eabdf75f97023e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/18/2020
ms.locfileid: "42733424"
---
# <a name="delete-windowsphone81trustedrootcertificate"></a><span data-ttu-id="9c710-103">Excluir windowsPhone81TrustedRootCertificate</span><span class="sxs-lookup"><span data-stu-id="9c710-103">Delete windowsPhone81TrustedRootCertificate</span></span>

> <span data-ttu-id="9c710-104">**Importante:** As APIs do Microsoft Graph na versão/beta estão sujeitas a alterações; Não há suporte para o uso de produção.</span><span class="sxs-lookup"><span data-stu-id="9c710-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9c710-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="9c710-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9c710-106">Exclui [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md).</span><span class="sxs-lookup"><span data-stu-id="9c710-106">Deletes a [windowsPhone81TrustedRootCertificate](../resources/intune-deviceconfig-windowsphone81trustedrootcertificate.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9c710-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="9c710-107">Prerequisites</span></span>
<span data-ttu-id="9c710-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="9c710-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9c710-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="9c710-110">Permission type</span></span>|<span data-ttu-id="9c710-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="9c710-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9c710-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="9c710-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9c710-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c710-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="9c710-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="9c710-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9c710-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="9c710-115">Not supported.</span></span>|
|<span data-ttu-id="9c710-116">Application</span><span class="sxs-lookup"><span data-stu-id="9c710-116">Application</span></span>|<span data-ttu-id="9c710-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9c710-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9c710-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="9c710-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
```

## <a name="request-headers"></a><span data-ttu-id="9c710-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="9c710-119">Request headers</span></span>
|<span data-ttu-id="9c710-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="9c710-120">Header</span></span>|<span data-ttu-id="9c710-121">Valor</span><span class="sxs-lookup"><span data-stu-id="9c710-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9c710-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="9c710-122">Authorization</span></span>|<span data-ttu-id="9c710-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="9c710-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9c710-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="9c710-124">Accept</span></span>|<span data-ttu-id="9c710-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9c710-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9c710-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="9c710-126">Request body</span></span>
<span data-ttu-id="9c710-127">Não forneça um corpo de solicitação para esse método.</span><span class="sxs-lookup"><span data-stu-id="9c710-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9c710-128">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c710-128">Response</span></span>
<span data-ttu-id="9c710-129">Se tiver êxito, este método retornará um código de resposta `204 No Content`.</span><span class="sxs-lookup"><span data-stu-id="9c710-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="9c710-130">Exemplo</span><span class="sxs-lookup"><span data-stu-id="9c710-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="9c710-131">Solicitação</span><span class="sxs-lookup"><span data-stu-id="9c710-131">Request</span></span>
<span data-ttu-id="9c710-132">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="9c710-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsPhone81VpnConfiguration/identityCertificate/microsoft.graph.windowsPhone81SCEPCertificateProfile/rootCertificate
```

### <a name="response"></a><span data-ttu-id="9c710-133">Resposta</span><span class="sxs-lookup"><span data-stu-id="9c710-133">Response</span></span>
<span data-ttu-id="9c710-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="9c710-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




