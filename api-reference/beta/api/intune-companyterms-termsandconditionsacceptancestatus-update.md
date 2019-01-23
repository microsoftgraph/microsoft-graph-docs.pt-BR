---
title: Atualizar termsAndConditionsAcceptanceStatus
description: Atualizar as propriedades de um objeto termsAndConditionsAcceptanceStatus.
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 548026bf033195364c0bda979f1501e62831ed13
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420539"
---
# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="7aaa6-103">Atualizar termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="7aaa6-103">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="7aaa6-104">**Importante:** APIs sob a versão /beta no Microsoft Graph estão sujeitos a alterações.</span><span class="sxs-lookup"><span data-stu-id="7aaa6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7aaa6-105">Não há suporte para o uso dessas APIs em aplicativos de produção.</span><span class="sxs-lookup"><span data-stu-id="7aaa6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7aaa6-106">**Observação:** A API do Microsoft Graph para Intune requer uma [licença de Intune ativa](https://go.microsoft.com/fwlink/?linkid=839381) para o inquilino.</span><span class="sxs-lookup"><span data-stu-id="7aaa6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7aaa6-107">Atualizar as propriedades de um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="7aaa6-107">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7aaa6-108">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="7aaa6-108">Prerequisites</span></span>
<span data-ttu-id="7aaa6-p102">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="7aaa6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7aaa6-111">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="7aaa6-111">Permission type</span></span>|<span data-ttu-id="7aaa6-112">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="7aaa6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7aaa6-113">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="7aaa6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7aaa6-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7aaa6-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="7aaa6-115">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="7aaa6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7aaa6-116">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7aaa6-116">Not supported.</span></span>|
|<span data-ttu-id="7aaa6-117">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="7aaa6-117">Application</span></span>|<span data-ttu-id="7aaa6-118">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="7aaa6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7aaa6-119">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="7aaa6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="7aaa6-120">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="7aaa6-120">Request headers</span></span>
|<span data-ttu-id="7aaa6-121">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="7aaa6-121">Header</span></span>|<span data-ttu-id="7aaa6-122">Valor</span><span class="sxs-lookup"><span data-stu-id="7aaa6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7aaa6-123">Autorização</span><span class="sxs-lookup"><span data-stu-id="7aaa6-123">Authorization</span></span>|<span data-ttu-id="7aaa6-124">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="7aaa6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7aaa6-125">Aceitar</span><span class="sxs-lookup"><span data-stu-id="7aaa6-125">Accept</span></span>|<span data-ttu-id="7aaa6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7aaa6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7aaa6-127">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="7aaa6-127">Request body</span></span>
<span data-ttu-id="7aaa6-128">No corpo da solicitação, forneça uma representação JSON do objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="7aaa6-128">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="7aaa6-129">A tabela a seguir mostra as propriedades que são necessárias ao criar [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span><span class="sxs-lookup"><span data-stu-id="7aaa6-129">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="7aaa6-130">Propriedade</span><span class="sxs-lookup"><span data-stu-id="7aaa6-130">Property</span></span>|<span data-ttu-id="7aaa6-131">Tipo</span><span class="sxs-lookup"><span data-stu-id="7aaa6-131">Type</span></span>|<span data-ttu-id="7aaa6-132">Descrição</span><span class="sxs-lookup"><span data-stu-id="7aaa6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7aaa6-133">id</span><span class="sxs-lookup"><span data-stu-id="7aaa6-133">id</span></span>|<span data-ttu-id="7aaa6-134">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7aaa6-134">String</span></span>|<span data-ttu-id="7aaa6-135">Identificador exclusivo da entidade.</span><span class="sxs-lookup"><span data-stu-id="7aaa6-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="7aaa6-136">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="7aaa6-136">userDisplayName</span></span>|<span data-ttu-id="7aaa6-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="7aaa6-137">String</span></span>|<span data-ttu-id="7aaa6-138">Nome de exibição do usuário cuja aceitação a entidade representa.</span><span class="sxs-lookup"><span data-stu-id="7aaa6-138">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="7aaa6-139">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="7aaa6-139">acceptedVersion</span></span>|<span data-ttu-id="7aaa6-140">Int32</span><span class="sxs-lookup"><span data-stu-id="7aaa6-140">Int32</span></span>|<span data-ttu-id="7aaa6-141">Número da versão mais recente dos T&C aceitos pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="7aaa6-141">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="7aaa6-142">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="7aaa6-142">acceptedDateTime</span></span>|<span data-ttu-id="7aaa6-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7aaa6-143">DateTimeOffset</span></span>|<span data-ttu-id="7aaa6-144">A data e a hora em que os termos foram aceitos pela última vez pelo usuário.</span><span class="sxs-lookup"><span data-stu-id="7aaa6-144">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="7aaa6-145">Resposta</span><span class="sxs-lookup"><span data-stu-id="7aaa6-145">Response</span></span>
<span data-ttu-id="7aaa6-146">Se tiver êxito, este método retornará um código de resposta `200 OK` e um objeto [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="7aaa6-146">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7aaa6-147">Exemplo</span><span class="sxs-lookup"><span data-stu-id="7aaa6-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="7aaa6-148">Solicitação</span><span class="sxs-lookup"><span data-stu-id="7aaa6-148">Request</span></span>
<span data-ttu-id="7aaa6-149">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="7aaa6-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="7aaa6-150">Resposta</span><span class="sxs-lookup"><span data-stu-id="7aaa6-150">Response</span></span>
<span data-ttu-id="7aaa6-p103">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="7aaa6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```




