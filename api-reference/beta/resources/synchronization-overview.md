---
title: Visão geral da API de sincronização do Azure AD
description: ') permite automatizar a criação, a manutenção e a remoção de identidades em aplicativos de nuvem (software como serviço ou SaaS) como o Dropbox, Salesforce, ServiceNow e muito mais. Você pode usar as APIs de sincronização no Microsoft Graph para gerenciar a sincronização de identidade de forma programática, incluindo:'
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c500eeb188461eaf245b6a9149421216cfaf2f43
ms.sourcegitcommit: 121c0fad692fb3c5c01dc051481b5249e4491b48
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 07/11/2019
ms.locfileid: "35620497"
---
# <a name="azure-ad-synchronization-api-overview"></a><span data-ttu-id="1f199-104">Visão geral da API de sincronização do Azure AD</span><span class="sxs-lookup"><span data-stu-id="1f199-104">Azure AD synchronization API overview</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f199-105">A sincronização de identidade do Azure Active Directory (Azure AD) (também chamada de "provisionamento") permite automatizar a criação, a manutenção e a remoção de identidades em aplicativos de nuvem (software como serviço ou SaaS) como o Dropbox, Salesforce, ServiceNow, e muito mais.</span><span class="sxs-lookup"><span data-stu-id="1f199-105">Azure Active Directory (Azure AD) identity synchronization (also called "provisioning") allows you to automate the creation, maintenance, and removal of identities in cloud (software as a service, or SaaS) applications such as Dropbox, Salesforce, ServiceNow, and more.</span></span> <span data-ttu-id="1f199-106">Você pode usar as APIs de sincronização no Microsoft Graph para gerenciar a sincronização de identidade de forma programática, incluindo:</span><span class="sxs-lookup"><span data-stu-id="1f199-106">You can use the synchronization APIs in Microsoft Graph to manage identity synchronization programmatically, including:</span></span>

- <span data-ttu-id="1f199-107">Criar, iniciar e interromper trabalhos de sincronização</span><span class="sxs-lookup"><span data-stu-id="1f199-107">Create, start, and stop synchronization jobs</span></span>
- <span data-ttu-id="1f199-108">Fazer alterações no esquema de sincronização para trabalhos</span><span class="sxs-lookup"><span data-stu-id="1f199-108">Make changes to the synchronization schema for jobs</span></span>
- <span data-ttu-id="1f199-109">Verificar o status de sincronização atual</span><span class="sxs-lookup"><span data-stu-id="1f199-109">Verify the current synchronization status</span></span> 

<span data-ttu-id="1f199-110">Para obter mais informações sobre sincronização no Azure AD, consulte:</span><span class="sxs-lookup"><span data-stu-id="1f199-110">For more information about synchronization in Azure AD, see:</span></span>

* [<span data-ttu-id="1f199-111">Automatizar o provisionamento de usuários e desprovisionamento para aplicativos SaaS com o Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="1f199-111">Automate user provisioning and deprovisioning to SaaS applications with Azure Active Directory</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-saas-app-provisioning)
* [<span data-ttu-id="1f199-112">Gerenciando o provisionamento de contas de usuário para aplicativos corporativos no portal do Azure</span><span class="sxs-lookup"><span data-stu-id="1f199-112">Managing user account provisioning for enterprise apps in the Azure portal</span></span>](https://docs.microsoft.com/en-us/azure/active-directory/active-directory-enterprise-apps-manage-provisioning)

<span data-ttu-id="1f199-113">Você também pode experimentar a API no [Explorador do Graph](https://developer.microsoft.com/graph/graph-explorer) em um locatário de exemplo ou seu próprio locatário.</span><span class="sxs-lookup"><span data-stu-id="1f199-113">You can also try the API in the [Graph Explorer](https://developer.microsoft.com/graph/graph-explorer) in a sample tenant or your own tenant.</span></span>

## <a name="synchronization-job"></a><span data-ttu-id="1f199-114">Trabalho de sincronização</span><span class="sxs-lookup"><span data-stu-id="1f199-114">Synchronization job</span></span>

<span data-ttu-id="1f199-115">Os trabalhos de sincronização realizam a sincronização periodicamente em segundo plano, pesquisando alterações em um diretório e empurrando-os para outro diretório.</span><span class="sxs-lookup"><span data-stu-id="1f199-115">Synchronization jobs perform synchronization by periodically running in the background, polling for changes in one directory, and pushing them to another directory.</span></span> <span data-ttu-id="1f199-116">O trabalho de sincronização é sempre específico para uma instância específica de um aplicativo em seu locatário.</span><span class="sxs-lookup"><span data-stu-id="1f199-116">The synchronization job is always specific to a particular instance of an application in your tenant.</span></span> <span data-ttu-id="1f199-117">Como parte da configuração do trabalho de sincronização, você precisa dar autorização para ler e gravar objetos no diretório de destino e personalizar o esquema de sincronização do trabalho.</span><span class="sxs-lookup"><span data-stu-id="1f199-117">As part of the synchronization job setup, you need to give authorization to read and write objects in your target directory, and customize the job's synchronization schema.</span></span>

<span data-ttu-id="1f199-118">Para obter mais informações, consulte [trabalho de sincronização](synchronization-synchronizationjob.md).</span><span class="sxs-lookup"><span data-stu-id="1f199-118">For more information, see [synchronization job](synchronization-synchronizationjob.md).</span></span>

## <a name="synchronization-schema"></a><span data-ttu-id="1f199-119">Esquema de sincronização</span><span class="sxs-lookup"><span data-stu-id="1f199-119">Synchronization schema</span></span>

<span data-ttu-id="1f199-120">O esquema de sincronização define quais objetos serão sincronizados e como eles serão sincronizados.</span><span class="sxs-lookup"><span data-stu-id="1f199-120">The synchronization schema defines what objects will be synchronized and how they will be synchronized.</span></span> <span data-ttu-id="1f199-121">O esquema de sincronização contém a maioria das informações de configuração de um determinado trabalho de sincronização.</span><span class="sxs-lookup"><span data-stu-id="1f199-121">The synchronization schema contains most of the setup information for a particular synchronization job.</span></span> <span data-ttu-id="1f199-122">Normalmente, você personalizará alguns dos mapeamentos de [atributo](synchronization-attributemapping.md)ou adicionará um [filtro de escopo](synchronization-filter.md) para sincronizar somente objetos que atendam a uma determinada condição.</span><span class="sxs-lookup"><span data-stu-id="1f199-122">Typically, you will customize some of the [attribute mappings](synchronization-attributemapping.md), or add a [scoping filter](synchronization-filter.md) to synchronize only objects that satisfy a certain condition.</span></span>

<span data-ttu-id="1f199-123">O esquema de sincronização inclui os seguintes componentes:</span><span class="sxs-lookup"><span data-stu-id="1f199-123">The synchronization schema includes the following components:</span></span>

- <span data-ttu-id="1f199-124">Definições de diretório</span><span class="sxs-lookup"><span data-stu-id="1f199-124">Directory definitions</span></span>
- <span data-ttu-id="1f199-125">Regras de sincronização</span><span class="sxs-lookup"><span data-stu-id="1f199-125">Synchronization rules</span></span>
- <span data-ttu-id="1f199-126">Mapeamentos de objetos</span><span class="sxs-lookup"><span data-stu-id="1f199-126">Object mappings</span></span>

<span data-ttu-id="1f199-127">Para obter mais informações, consulte [Synchronization Schema](synchronization-synchronizationschema.md).</span><span class="sxs-lookup"><span data-stu-id="1f199-127">For more information, see [synchronization schema](synchronization-synchronizationschema.md).</span></span>

## <a name="synchronization-template"></a><span data-ttu-id="1f199-128">Modelo de sincronização</span><span class="sxs-lookup"><span data-stu-id="1f199-128">Synchronization template</span></span>

<span data-ttu-id="1f199-129">O modelo de sincronização fornece configurações de sincronização pré-configuradas para um aplicativo específico.</span><span class="sxs-lookup"><span data-stu-id="1f199-129">The synchronization template provides pre-configured synchronization settings for a particular application.</span></span> <span data-ttu-id="1f199-130">Essas configurações (mais importante, [esquema de sincronização](synchronization-synchronizationschema.md)) serão usadas por padrão para qualquer [trabalho de sincronização](synchronization-synchronizationjob.md) baseado no modelo.</span><span class="sxs-lookup"><span data-stu-id="1f199-130">These settings (most importantly, [synchronization schema](synchronization-synchronizationschema.md)) will be used by default for any [synchronization job](synchronization-synchronizationjob.md) that is based on the template.</span></span> <span data-ttu-id="1f199-131">Os modelos são especificados pelo desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1f199-131">Templates are specified by the application developer.</span></span>

<span data-ttu-id="1f199-132">Para obter mais informações, consulte [modelo de sincronização](synchronization-synchronizationtemplate.md).</span><span class="sxs-lookup"><span data-stu-id="1f199-132">For more information, see [synchronization template](synchronization-synchronizationtemplate.md).</span></span>

## <a name="working-with-the-synchronization-api"></a><span data-ttu-id="1f199-133">Trabalhar com a API de sincronização</span><span class="sxs-lookup"><span data-stu-id="1f199-133">Working with the synchronization API</span></span>

<span data-ttu-id="1f199-134">O trabalho com a API de sincronização envolve principalmente o acesso aos recursos do [synchronizationJob](synchronization-synchronizationjob.md) e do [synchronizationSchema](synchronization-synchronizationschema.md) .</span><span class="sxs-lookup"><span data-stu-id="1f199-134">Working with synchronization API primarily involves accessing the [synchronizationJob](synchronization-synchronizationjob.md) and [synchronizationSchema](synchronization-synchronizationschema.md) resources.</span></span> <span data-ttu-id="1f199-135">Para localizar o recurso [synchronizationJob](synchronization-synchronizationjob.md) , você precisa saber a ID do objeto de entidade de serviço ao qual o trabalho de sincronização pertence.</span><span class="sxs-lookup"><span data-stu-id="1f199-135">To find your [synchronizationJob](synchronization-synchronizationjob.md) resource, you need to know the ID of the service principal object that the synchronization job belongs to.</span></span> <span data-ttu-id="1f199-136">Os exemplos a seguir mostram como trabalhar com os recursos **synchronizationJob** e **synchronizationSchema** .</span><span class="sxs-lookup"><span data-stu-id="1f199-136">The following examples show you how to work with the **synchronizationJob** and **synchronizationSchema** resources.</span></span>

### <a name="authorization"></a><span data-ttu-id="1f199-137">Autorização</span><span class="sxs-lookup"><span data-stu-id="1f199-137">Authorization</span></span>

<span data-ttu-id="1f199-138">A API de sincronização do Azure AD usa o OAuth 2,0 para autorização.</span><span class="sxs-lookup"><span data-stu-id="1f199-138">The Azure AD synchronization API uses OAuth 2.0 for authorization.</span></span> <span data-ttu-id="1f199-139">Antes de fazer qualquer solicitação para a API, você precisa obter um token de acesso.</span><span class="sxs-lookup"><span data-stu-id="1f199-139">Before making any requests to the API, you need to get an access token.</span></span> <span data-ttu-id="1f199-140">Para obter mais informações, consulte [obter tokens de acesso para chamar o Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span><span class="sxs-lookup"><span data-stu-id="1f199-140">For more information, see [Get access tokens to call Microsoft Graph](https://developer.microsoft.com/graph/docs/concepts/auth_overview).</span></span> <span data-ttu-id="1f199-141">Para acessar os recursos de sincronização, seu aplicativo precisa de permissões de Directory. ReadWrite. All.</span><span class="sxs-lookup"><span data-stu-id="1f199-141">To access synchronization resources, your application needs Directory.ReadWrite.All permissions.</span></span> <span data-ttu-id="1f199-142">Para obter mais informações, consulte [Directory Permissions](/graph/permissions-reference#directory-permissions).</span><span class="sxs-lookup"><span data-stu-id="1f199-142">For more information, see [Directory permissions](/graph/permissions-reference#directory-permissions).</span></span>

### <a name="find-the-service-principal-object-by-display-name"></a><span data-ttu-id="1f199-143">Localizar o objeto de entidade de serviço por nome de exibição</span><span class="sxs-lookup"><span data-stu-id="1f199-143">Find the service principal object by display name</span></span>

<span data-ttu-id="1f199-144">O exemplo a seguir mostra como localizar o objeto de entidade de serviço por nome de exibição.</span><span class="sxs-lookup"><span data-stu-id="1f199-144">The following example shows how to find service principal object by display name.</span></span>

<span data-ttu-id="1f199-145">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="1f199-145">**Request**</span></span> 

<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=startswith(displayName, 'salesforce')
```

<span data-ttu-id="1f199-146">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="1f199-146">**Response**</span></span>

<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "value": [
    {
        "id": "bc0dc311-87df-48ac-91b1-259bd2c3a31c",
        "appId": "f7808c5e-cb57-4e37-8094-406d302c0f8d",
        "displayName": "Salesforce"
    },
    {
        "id": "d813d7d7-0f41-4edc-b284-d0dfaf399d15",
        "appId": "219561ee-1480-4c67-9aa6-63d861fae3ef",
        "displayName": "salesforce 3"
    }
    ]
}
```

### <a name="find-the-service-principal-object-by-app-id"></a><span data-ttu-id="1f199-147">Localizar o objeto de entidade de serviço por ID de aplicativo</span><span class="sxs-lookup"><span data-stu-id="1f199-147">Find the service principal object by app ID</span></span>

<span data-ttu-id="1f199-148">O exemplo a seguir mostra como localizar o objeto de entidade de serviço por ID de aplicativo.</span><span class="sxs-lookup"><span data-stu-id="1f199-148">The following example shows how to find the service principal object by app ID.</span></span>

<span data-ttu-id="1f199-149">**Pedir** 
</span><span class="sxs-lookup"><span data-stu-id="1f199-149">**Request** 
</span></span><!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals?$select=id,appId,displayName&$filter=AppId eq '219561ee-1480-4c67-9aa6-63d861fae3ef'
```

<span data-ttu-id="1f199-150">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="1f199-150">**Response**</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "value": [
        {
            "id": "d813d7d7-0f41-4edc-b284-d0dfaf399d15",
            "appId": "219561ee-1480-4c67-9aa6-63d861fae3ef",
            "displayName": "salesforce 3"
        }
    ]
}
```

### <a name="list-existing-synchronization-jobs"></a><span data-ttu-id="1f199-151">Listar trabalhos de sincronização existentes</span><span class="sxs-lookup"><span data-stu-id="1f199-151">List existing synchronization jobs</span></span>

<span data-ttu-id="1f199-152">O exemplo a seguir mostra como listar os trabalhos de sincronização existentes.</span><span class="sxs-lookup"><span data-stu-id="1f199-152">The following example shows you how to list existing synchronization jobs.</span></span>

<span data-ttu-id="1f199-153">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="1f199-153">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs
GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs
```

<span data-ttu-id="1f199-154">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="1f199-154">**Response**</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "value": [
        {
            "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
            "templateId": "SfSandboxOutDelta",
            "schedule": {
                "expiration": null,
                "interval": "PT20M",
                "state": "Active"
            },
            "status": {}
        }
    ]
}
```

### <a name="get-synchronization-job-status"></a><span data-ttu-id="1f199-155">Obter o status do trabalho de sincronização</span><span class="sxs-lookup"><span data-stu-id="1f199-155">Get synchronization job status</span></span>
<span data-ttu-id="1f199-156">O exemplo a seguir mostra como obter o status de um trabalho de sincronização.</span><span class="sxs-lookup"><span data-stu-id="1f199-156">The following example shows you how to get the status of a synchronization job.</span></span>

<span data-ttu-id="1f199-157">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="1f199-157">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}

GET https://graph.microsoft.com/beta/servicePrincipals/60443998-8cf7-4e61-b05c-a53b658cb5e1/synchronization/jobs/SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa
```

<span data-ttu-id="1f199-158">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="1f199-158">**Response**</span></span>
<!-- { "blockType": "ignored" } -->
```http
    HTTP/1.1 200 OK
    {
        "id": "SfSandboxOutDelta.e4bbf44533ea4eabb17027f3a92e92aa",
        "templateId": "SfSandboxOutDelta",
        "schedule": {
            "expiration": null,
            "interval": "PT20M",
            "state": "Active"
        },
        "status": {}
    }
```

### <a name="get-synchronization-schema"></a><span data-ttu-id="1f199-159">Obter esquema de sincronização</span><span class="sxs-lookup"><span data-stu-id="1f199-159">Get synchronization schema</span></span>
<span data-ttu-id="1f199-160">O exemplo a seguir mostra como obter o esquema de sincronização.</span><span class="sxs-lookup"><span data-stu-id="1f199-160">The following example shows you how to get the synchronization schema.</span></span>

<span data-ttu-id="1f199-161">**Solicitação**</span><span class="sxs-lookup"><span data-stu-id="1f199-161">**Request**</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/synchronization/jobs/{jobId}/schema
```

<span data-ttu-id="1f199-162">**Resposta**</span><span class="sxs-lookup"><span data-stu-id="1f199-162">**Response**</span></span>
<!-- { "blockType": "ignored" } -->
```http
HTTP/1.1 200 OK
{
    "directories": [],
    "synchronizationRules": []
}
```
## <a name="see-also"></a><span data-ttu-id="1f199-163">Confira também</span><span class="sxs-lookup"><span data-stu-id="1f199-163">See also</span></span>

* [<span data-ttu-id="1f199-164">Configurar a sincronização com atributos de extensão de diretório</span><span class="sxs-lookup"><span data-stu-id="1f199-164">Configure synchronization with directory extension attributes</span></span>](../resources/synchronization-configure-with-directory-extension-attributes.md)
* [<span data-ttu-id="1f199-165">Configurar a sincronização com atributos de destino personalizados</span><span class="sxs-lookup"><span data-stu-id="1f199-165">Configure synchronization with custom target attributes</span></span>](../resources/synchronization-configure-with-custom-target-attributes.md)



