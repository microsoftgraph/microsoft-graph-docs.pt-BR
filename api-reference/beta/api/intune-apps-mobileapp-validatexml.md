---
title: Ação validateXml
description: Ainda não documentado
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a6094bb2c8c9c77e080a3795137a6b90544806f0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143378"
---
# <a name="validatexml-action"></a><span data-ttu-id="7c9d8-103">Ação validateXml</span><span class="sxs-lookup"><span data-stu-id="7c9d8-103">validateXml action</span></span>

<span data-ttu-id="7c9d8-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7c9d8-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7c9d8-105">**Importante:** As APIs do Microsoft Graph na versão /beta estão sujeitas a alterações; não há suporte para uso de produção.</span><span class="sxs-lookup"><span data-stu-id="7c9d8-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7c9d8-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7c9d8-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c9d8-107">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7c9d8-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c9d8-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7c9d8-108">Prerequisites</span></span>
<span data-ttu-id="7c9d8-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7c9d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7c9d8-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7c9d8-111">Permission type</span></span>|<span data-ttu-id="7c9d8-112">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7c9d8-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c9d8-113">Delegada (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7c9d8-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c9d8-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c9d8-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7c9d8-115">Delegada (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7c9d8-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c9d8-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7c9d8-116">Not supported.</span></span>|
|<span data-ttu-id="7c9d8-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7c9d8-117">Application</span></span>|<span data-ttu-id="7c9d8-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7c9d8-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c9d8-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7c9d8-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/validateXml
```

## <a name="request-headers"></a><span data-ttu-id="7c9d8-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7c9d8-120">Request headers</span></span>
|<span data-ttu-id="7c9d8-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7c9d8-121">Header</span></span>|<span data-ttu-id="7c9d8-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7c9d8-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c9d8-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7c9d8-123">Authorization</span></span>|<span data-ttu-id="7c9d8-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7c9d8-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c9d8-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7c9d8-125">Accept</span></span>|<span data-ttu-id="7c9d8-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c9d8-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c9d8-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7c9d8-127">Request body</span></span>
<span data-ttu-id="7c9d8-128">No corpo da solicitação, forneça uma representação JSON dos parâmetros.</span><span class="sxs-lookup"><span data-stu-id="7c9d8-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7c9d8-129">A tabela a seguir mostra os parâmetros que podem ser usados com esta ação.</span><span class="sxs-lookup"><span data-stu-id="7c9d8-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7c9d8-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7c9d8-130">Property</span></span>|<span data-ttu-id="7c9d8-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7c9d8-131">Type</span></span>|<span data-ttu-id="7c9d8-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7c9d8-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7c9d8-133">officeConfigurationXml</span><span class="sxs-lookup"><span data-stu-id="7c9d8-133">officeConfigurationXml</span></span>|<span data-ttu-id="7c9d8-134">Binário</span><span class="sxs-lookup"><span data-stu-id="7c9d8-134">Binary</span></span>|<span data-ttu-id="7c9d8-135">Ainda não documentado</span><span class="sxs-lookup"><span data-stu-id="7c9d8-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7c9d8-136">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c9d8-136">Response</span></span>
<span data-ttu-id="7c9d8-137">Se tiver êxito, esta ação retornará um código de resposta `200 OK` e uma cadeia de caracteres no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7c9d8-137">If successful, this action returns a `200 OK` response code and a String in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c9d8-138">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7c9d8-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c9d8-139">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7c9d8-139">Request</span></span>
<span data-ttu-id="7c9d8-140">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7c9d8-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/validateXml

Content-type: application/json
Content-length: 68

{
  "officeConfigurationXml": "b2ZmaWNlQ29uZmlndXJhdGlvblhtbA=="
}
```

### <a name="response"></a><span data-ttu-id="7c9d8-141">Resposta</span><span class="sxs-lookup"><span data-stu-id="7c9d8-141">Response</span></span>
<span data-ttu-id="7c9d8-p102">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7c9d8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 37

{
  "value": "Validate Xml value"
}
```




