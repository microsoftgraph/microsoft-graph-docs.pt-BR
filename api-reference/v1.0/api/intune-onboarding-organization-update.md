---
title: Atualize a organização
description: Atualizar as propriedades de um objeto organização.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b66eea4b04f21f85aa38b9777a17cb73e87fe6fc
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52751458"
---
# <a name="update-organization"></a><span data-ttu-id="7cf88-103">Atualize a organização</span><span class="sxs-lookup"><span data-stu-id="7cf88-103">Update organization</span></span>

<span data-ttu-id="7cf88-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7cf88-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7cf88-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="7cf88-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7cf88-106">Atualizar as propriedades de um objeto [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="7cf88-106">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7cf88-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7cf88-107">Prerequisites</span></span>
<span data-ttu-id="7cf88-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="7cf88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cf88-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7cf88-110">Permission type</span></span>|<span data-ttu-id="7cf88-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="7cf88-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cf88-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7cf88-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7cf88-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cf88-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7cf88-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7cf88-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cf88-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7cf88-115">Not supported.</span></span>|
|<span data-ttu-id="7cf88-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7cf88-116">Application</span></span>|<span data-ttu-id="7cf88-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7cf88-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cf88-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7cf88-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="7cf88-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7cf88-119">Request headers</span></span>
|<span data-ttu-id="7cf88-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7cf88-120">Header</span></span>|<span data-ttu-id="7cf88-121">Valor</span><span class="sxs-lookup"><span data-stu-id="7cf88-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7cf88-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="7cf88-122">Authorization</span></span>|<span data-ttu-id="7cf88-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7cf88-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7cf88-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7cf88-124">Accept</span></span>|<span data-ttu-id="7cf88-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7cf88-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cf88-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7cf88-126">Request body</span></span>
<span data-ttu-id="7cf88-127">No corpo da solicitação, forneça uma representação JSON do objeto [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="7cf88-127">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="7cf88-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="7cf88-128">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="7cf88-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7cf88-129">Property</span></span>|<span data-ttu-id="7cf88-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="7cf88-130">Type</span></span>|<span data-ttu-id="7cf88-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="7cf88-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7cf88-132">id</span><span class="sxs-lookup"><span data-stu-id="7cf88-132">id</span></span>|<span data-ttu-id="7cf88-133">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7cf88-133">String</span></span>|<span data-ttu-id="7cf88-134">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="7cf88-134">The GUID for the object.</span></span>|
|<span data-ttu-id="7cf88-135">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="7cf88-135">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="7cf88-136">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="7cf88-136">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="7cf88-137">Define autoridade de gerenciamento de dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="7cf88-137">Mobile device management authority.</span></span> <span data-ttu-id="7cf88-138">Os valores possíveis são: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="7cf88-138">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|



## <a name="response"></a><span data-ttu-id="7cf88-139">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cf88-139">Response</span></span>
<span data-ttu-id="7cf88-140">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [organization](../resources/intune-onboarding-organization.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7cf88-140">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cf88-141">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7cf88-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="7cf88-142">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7cf88-142">Request</span></span>
<span data-ttu-id="7cf88-143">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7cf88-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/organization/{organizationId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.organization",
  "mobileDeviceManagementAuthority": "intune"
}
```

### <a name="response"></a><span data-ttu-id="7cf88-144">Resposta</span><span class="sxs-lookup"><span data-stu-id="7cf88-144">Response</span></span>
<span data-ttu-id="7cf88-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7cf88-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 151

{
  "@odata.type": "#microsoft.graph.organization",
  "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
  "mobileDeviceManagementAuthority": "intune"
}
```




