---
title: Atualize a organização
description: Atualizar as propriedades de um objeto organização.
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b639ff8d3a2d043bd001f160a0c04ca97a11dbba
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 02/26/2019
ms.locfileid: "30258482"
---
# <a name="update-organization"></a><span data-ttu-id="4a5df-103">Atualize a organização</span><span class="sxs-lookup"><span data-stu-id="4a5df-103">Update organization</span></span>

> <span data-ttu-id="4a5df-104">**Observação:** A API do Microsoft Graph para Intune requer uma [licença do Active Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="4a5df-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4a5df-105">Atualizar as propriedades de um objeto [organização](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="4a5df-105">Update the properties of a [organization](../resources/intune-onboarding-organization.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4a5df-106">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="4a5df-106">Prerequisites</span></span>
<span data-ttu-id="4a5df-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="4a5df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="4a5df-109">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="4a5df-109">Permission type</span></span>|<span data-ttu-id="4a5df-110">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="4a5df-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4a5df-111">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="4a5df-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4a5df-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4a5df-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4a5df-113">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="4a5df-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4a5df-114">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a5df-114">Not supported.</span></span>|
|<span data-ttu-id="4a5df-115">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="4a5df-115">Application</span></span>|<span data-ttu-id="4a5df-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="4a5df-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4a5df-117">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="4a5df-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="4a5df-118">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="4a5df-118">Request headers</span></span>
|<span data-ttu-id="4a5df-119">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="4a5df-119">Header</span></span>|<span data-ttu-id="4a5df-120">Valor</span><span class="sxs-lookup"><span data-stu-id="4a5df-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4a5df-121">Autorização</span><span class="sxs-lookup"><span data-stu-id="4a5df-121">Authorization</span></span>|<span data-ttu-id="4a5df-122">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="4a5df-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4a5df-123">Aceitar</span><span class="sxs-lookup"><span data-stu-id="4a5df-123">Accept</span></span>|<span data-ttu-id="4a5df-124">application/json</span><span class="sxs-lookup"><span data-stu-id="4a5df-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4a5df-125">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="4a5df-125">Request body</span></span>
<span data-ttu-id="4a5df-126">No corpo da solicitação, forneça uma representação JSON do objeto [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="4a5df-126">In the request body, supply a JSON representation for the [organization](../resources/intune-onboarding-organization.md) object.</span></span>

<span data-ttu-id="4a5df-127">A tabela a seguir mostra as propriedades que são necessárias ao criar [organization](../resources/intune-onboarding-organization.md).</span><span class="sxs-lookup"><span data-stu-id="4a5df-127">The following table shows the properties that are required when you create the [organization](../resources/intune-onboarding-organization.md).</span></span>

|<span data-ttu-id="4a5df-128">Propriedade</span><span class="sxs-lookup"><span data-stu-id="4a5df-128">Property</span></span>|<span data-ttu-id="4a5df-129">Tipo</span><span class="sxs-lookup"><span data-stu-id="4a5df-129">Type</span></span>|<span data-ttu-id="4a5df-130">Descrição</span><span class="sxs-lookup"><span data-stu-id="4a5df-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4a5df-131">id</span><span class="sxs-lookup"><span data-stu-id="4a5df-131">id</span></span>|<span data-ttu-id="4a5df-132">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="4a5df-132">String</span></span>|<span data-ttu-id="4a5df-133">O GUID do objeto.</span><span class="sxs-lookup"><span data-stu-id="4a5df-133">The GUID for the object.</span></span>|
|<span data-ttu-id="4a5df-134">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="4a5df-134">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="4a5df-135">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="4a5df-135">mdmAuthority</span></span>](../resources/intune-onboarding-mdmauthority.md)|<span data-ttu-id="4a5df-136">Define autoridade de gerenciamento de dispositivo móvel.</span><span class="sxs-lookup"><span data-stu-id="4a5df-136">Mobile device management authority.</span></span> <span data-ttu-id="4a5df-137">Os valores possíveis são: `unknown`, `intune`, `sccm`, `office365`.</span><span class="sxs-lookup"><span data-stu-id="4a5df-137">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|



## <a name="response"></a><span data-ttu-id="4a5df-138">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a5df-138">Response</span></span>
<span data-ttu-id="4a5df-139">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [organization](../resources/intune-onboarding-organization.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="4a5df-139">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune-onboarding-organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4a5df-140">Exemplo</span><span class="sxs-lookup"><span data-stu-id="4a5df-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="4a5df-141">Solicitação</span><span class="sxs-lookup"><span data-stu-id="4a5df-141">Request</span></span>
<span data-ttu-id="4a5df-142">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="4a5df-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/organization/{organizationId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.organization",
  "mobileDeviceManagementAuthority": "intune"
}
```

### <a name="response"></a><span data-ttu-id="4a5df-143">Resposta</span><span class="sxs-lookup"><span data-stu-id="4a5df-143">Response</span></span>
<span data-ttu-id="4a5df-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="4a5df-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



