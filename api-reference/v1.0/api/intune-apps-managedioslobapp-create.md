---
title: Criar managedIOSLobApp
description: Cria um novo objeto managedIOSLobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 36e2c66cdd98b3e29a2102a9f50c8a74d11c7a22
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 09/18/2020
ms.locfileid: "48025834"
---
# <a name="create-managedioslobapp"></a><span data-ttu-id="58a92-103">Criar managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="58a92-103">Create managedIOSLobApp</span></span>

<span data-ttu-id="58a92-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="58a92-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="58a92-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="58a92-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="58a92-106">Cria um novo objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="58a92-106">Create a new [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="58a92-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="58a92-107">Prerequisites</span></span>
<span data-ttu-id="58a92-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="58a92-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="58a92-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="58a92-110">Permission type</span></span>|<span data-ttu-id="58a92-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="58a92-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="58a92-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="58a92-112">Delegated (work or school account)</span></span>|<span data-ttu-id="58a92-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58a92-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="58a92-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="58a92-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="58a92-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="58a92-115">Not supported.</span></span>|
|<span data-ttu-id="58a92-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="58a92-116">Application</span></span>|<span data-ttu-id="58a92-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="58a92-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="58a92-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="58a92-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="58a92-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="58a92-119">Request headers</span></span>
|<span data-ttu-id="58a92-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="58a92-120">Header</span></span>|<span data-ttu-id="58a92-121">Valor</span><span class="sxs-lookup"><span data-stu-id="58a92-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="58a92-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="58a92-122">Authorization</span></span>|<span data-ttu-id="58a92-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="58a92-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="58a92-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="58a92-124">Accept</span></span>|<span data-ttu-id="58a92-125">application/json</span><span class="sxs-lookup"><span data-stu-id="58a92-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="58a92-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="58a92-126">Request body</span></span>
<span data-ttu-id="58a92-127">No corpo da solicitação, forneça uma representação JSON do objeto managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="58a92-127">In the request body, supply a JSON representation for the managedIOSLobApp object.</span></span>

<span data-ttu-id="58a92-128">A tabela a seguir mostra as propriedades obrigatórias ao criar managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="58a92-128">The following table shows the properties that are required when you create the managedIOSLobApp.</span></span>

|<span data-ttu-id="58a92-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="58a92-129">Property</span></span>|<span data-ttu-id="58a92-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="58a92-130">Type</span></span>|<span data-ttu-id="58a92-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="58a92-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="58a92-132">id</span><span class="sxs-lookup"><span data-stu-id="58a92-132">id</span></span>|<span data-ttu-id="58a92-133">String</span><span class="sxs-lookup"><span data-stu-id="58a92-133">String</span></span>|<span data-ttu-id="58a92-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="58a92-134">Key of the entity.</span></span> <span data-ttu-id="58a92-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58a92-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58a92-136">displayName</span><span class="sxs-lookup"><span data-stu-id="58a92-136">displayName</span></span>|<span data-ttu-id="58a92-137">String</span><span class="sxs-lookup"><span data-stu-id="58a92-137">String</span></span>|<span data-ttu-id="58a92-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="58a92-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="58a92-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58a92-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58a92-140">description</span><span class="sxs-lookup"><span data-stu-id="58a92-140">description</span></span>|<span data-ttu-id="58a92-141">String</span><span class="sxs-lookup"><span data-stu-id="58a92-141">String</span></span>|<span data-ttu-id="58a92-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="58a92-142">The description of the app.</span></span> <span data-ttu-id="58a92-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58a92-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58a92-144">publicador</span><span class="sxs-lookup"><span data-stu-id="58a92-144">publisher</span></span>|<span data-ttu-id="58a92-145">String</span><span class="sxs-lookup"><span data-stu-id="58a92-145">String</span></span>|<span data-ttu-id="58a92-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="58a92-146">The publisher of the app.</span></span> <span data-ttu-id="58a92-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58a92-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58a92-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="58a92-148">largeIcon</span></span>|[<span data-ttu-id="58a92-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="58a92-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="58a92-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="58a92-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="58a92-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58a92-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58a92-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="58a92-152">createdDateTime</span></span>|<span data-ttu-id="58a92-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58a92-153">DateTimeOffset</span></span>|<span data-ttu-id="58a92-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="58a92-154">The date and time the app was created.</span></span> <span data-ttu-id="58a92-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58a92-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58a92-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="58a92-156">lastModifiedDateTime</span></span>|<span data-ttu-id="58a92-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58a92-157">DateTimeOffset</span></span>|<span data-ttu-id="58a92-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="58a92-158">The date and time the app was last modified.</span></span> <span data-ttu-id="58a92-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58a92-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58a92-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="58a92-160">isFeatured</span></span>|<span data-ttu-id="58a92-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="58a92-161">Boolean</span></span>|<span data-ttu-id="58a92-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58a92-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58a92-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="58a92-163">privacyInformationUrl</span></span>|<span data-ttu-id="58a92-164">String</span><span class="sxs-lookup"><span data-stu-id="58a92-164">String</span></span>|<span data-ttu-id="58a92-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="58a92-165">The privacy statement Url.</span></span> <span data-ttu-id="58a92-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58a92-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58a92-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="58a92-167">informationUrl</span></span>|<span data-ttu-id="58a92-168">String</span><span class="sxs-lookup"><span data-stu-id="58a92-168">String</span></span>|<span data-ttu-id="58a92-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="58a92-169">The more information Url.</span></span> <span data-ttu-id="58a92-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58a92-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58a92-171">proprietário</span><span class="sxs-lookup"><span data-stu-id="58a92-171">owner</span></span>|<span data-ttu-id="58a92-172">String</span><span class="sxs-lookup"><span data-stu-id="58a92-172">String</span></span>|<span data-ttu-id="58a92-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="58a92-173">The owner of the app.</span></span> <span data-ttu-id="58a92-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58a92-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58a92-175">developer</span><span class="sxs-lookup"><span data-stu-id="58a92-175">developer</span></span>|<span data-ttu-id="58a92-176">String</span><span class="sxs-lookup"><span data-stu-id="58a92-176">String</span></span>|<span data-ttu-id="58a92-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="58a92-177">The developer of the app.</span></span> <span data-ttu-id="58a92-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58a92-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58a92-179">notes</span><span class="sxs-lookup"><span data-stu-id="58a92-179">notes</span></span>|<span data-ttu-id="58a92-180">String</span><span class="sxs-lookup"><span data-stu-id="58a92-180">String</span></span>|<span data-ttu-id="58a92-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="58a92-181">Notes for the app.</span></span> <span data-ttu-id="58a92-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="58a92-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="58a92-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="58a92-183">publishingState</span></span>|[<span data-ttu-id="58a92-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="58a92-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="58a92-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="58a92-185">The publishing state for the app.</span></span> <span data-ttu-id="58a92-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="58a92-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="58a92-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="58a92-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="58a92-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="58a92-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="58a92-189">appAvailability</span><span class="sxs-lookup"><span data-stu-id="58a92-189">appAvailability</span></span>|[<span data-ttu-id="58a92-190">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="58a92-190">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="58a92-191">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="58a92-191">The Application's availability.</span></span> <span data-ttu-id="58a92-192">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="58a92-192">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="58a92-193">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="58a92-193">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="58a92-194">version</span><span class="sxs-lookup"><span data-stu-id="58a92-194">version</span></span>|<span data-ttu-id="58a92-195">String</span><span class="sxs-lookup"><span data-stu-id="58a92-195">String</span></span>|<span data-ttu-id="58a92-196">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="58a92-196">The Application's version.</span></span> <span data-ttu-id="58a92-197">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="58a92-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="58a92-198">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="58a92-198">committedContentVersion</span></span>|<span data-ttu-id="58a92-199">String</span><span class="sxs-lookup"><span data-stu-id="58a92-199">String</span></span>|<span data-ttu-id="58a92-200">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="58a92-200">The internal committed content version.</span></span> <span data-ttu-id="58a92-201">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="58a92-201">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="58a92-202">fileName</span><span class="sxs-lookup"><span data-stu-id="58a92-202">fileName</span></span>|<span data-ttu-id="58a92-203">String</span><span class="sxs-lookup"><span data-stu-id="58a92-203">String</span></span>|<span data-ttu-id="58a92-204">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="58a92-204">The name of the main Lob application file.</span></span> <span data-ttu-id="58a92-205">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="58a92-205">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="58a92-206">size</span><span class="sxs-lookup"><span data-stu-id="58a92-206">size</span></span>|<span data-ttu-id="58a92-207">Int64</span><span class="sxs-lookup"><span data-stu-id="58a92-207">Int64</span></span>|<span data-ttu-id="58a92-208">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="58a92-208">The total size, including all uploaded files.</span></span> <span data-ttu-id="58a92-209">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="58a92-209">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="58a92-210">bundleId</span><span class="sxs-lookup"><span data-stu-id="58a92-210">bundleId</span></span>|<span data-ttu-id="58a92-211">String</span><span class="sxs-lookup"><span data-stu-id="58a92-211">String</span></span>|<span data-ttu-id="58a92-212">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="58a92-212">The Identity Name.</span></span>|
|<span data-ttu-id="58a92-213">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="58a92-213">applicableDeviceType</span></span>|[<span data-ttu-id="58a92-214">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="58a92-214">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="58a92-215">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="58a92-215">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="58a92-216">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="58a92-216">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="58a92-217">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="58a92-217">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="58a92-218">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="58a92-218">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="58a92-219">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="58a92-219">expirationDateTime</span></span>|<span data-ttu-id="58a92-220">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="58a92-220">DateTimeOffset</span></span>|<span data-ttu-id="58a92-221">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="58a92-221">The expiration time.</span></span>|
|<span data-ttu-id="58a92-222">versionNumber</span><span class="sxs-lookup"><span data-stu-id="58a92-222">versionNumber</span></span>|<span data-ttu-id="58a92-223">String</span><span class="sxs-lookup"><span data-stu-id="58a92-223">String</span></span>|<span data-ttu-id="58a92-224">O número de versão do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="58a92-224">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="58a92-225">buildNumber</span><span class="sxs-lookup"><span data-stu-id="58a92-225">buildNumber</span></span>|<span data-ttu-id="58a92-226">String</span><span class="sxs-lookup"><span data-stu-id="58a92-226">String</span></span>|<span data-ttu-id="58a92-227">O número de build do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="58a92-227">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="58a92-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="58a92-228">Response</span></span>
<span data-ttu-id="58a92-229">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="58a92-229">If successful, this method returns a `201 Created` response code and a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="58a92-230">Exemplo</span><span class="sxs-lookup"><span data-stu-id="58a92-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="58a92-231">Solicitação</span><span class="sxs-lookup"><span data-stu-id="58a92-231">Request</span></span>
<span data-ttu-id="58a92-232">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="58a92-232">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
Content-type: application/json
Content-length: 1307

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```

### <a name="response"></a><span data-ttu-id="58a92-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="58a92-233">Response</span></span>
<span data-ttu-id="58a92-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="58a92-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1479

{
  "@odata.type": "#microsoft.graph.managedIOSLobApp",
  "id": "8f59792d-792d-8f59-2d79-598f2d79598f",
  "displayName": "Display Name value",
  "description": "Description value",
  "publisher": "Publisher value",
  "largeIcon": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "isFeatured": true,
  "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
  "informationUrl": "https://example.com/informationUrl/",
  "owner": "Owner value",
  "developer": "Developer value",
  "notes": "Notes value",
  "publishingState": "processing",
  "appAvailability": "lineOfBusiness",
  "version": "Version value",
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "bundleId": "Bundle Id value",
  "applicableDeviceType": {
    "@odata.type": "microsoft.graph.iosDeviceType",
    "iPad": true,
    "iPhoneAndIPod": true
  },
  "minimumSupportedOperatingSystem": {
    "@odata.type": "microsoft.graph.iosMinimumOperatingSystem",
    "v8_0": true,
    "v9_0": true,
    "v10_0": true,
    "v11_0": true,
    "v12_0": true,
    "v13_0": true
  },
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "versionNumber": "Version Number value",
  "buildNumber": "Build Number value"
}
```









