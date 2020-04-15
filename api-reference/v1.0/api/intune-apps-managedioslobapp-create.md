---
title: Criar managedIOSLobApp
description: Cria um novo objeto managedIOSLobApp.
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 63966fd441149f55fe635c0fbff2c2480719cd3a
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 04/14/2020
ms.locfileid: "43442639"
---
# <a name="create-managedioslobapp"></a><span data-ttu-id="3b335-103">Criar managedIOSLobApp</span><span class="sxs-lookup"><span data-stu-id="3b335-103">Create managedIOSLobApp</span></span>

<span data-ttu-id="3b335-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3b335-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3b335-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="3b335-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3b335-106">Cria um novo objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b335-106">Create a new [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3b335-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="3b335-107">Prerequisites</span></span>
<span data-ttu-id="3b335-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/concepts/permissions-reference.md).</span><span class="sxs-lookup"><span data-stu-id="3b335-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3b335-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="3b335-110">Permission type</span></span>|<span data-ttu-id="3b335-111">Permissões (de privilégios máximos a mínimos)</span><span class="sxs-lookup"><span data-stu-id="3b335-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b335-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="3b335-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3b335-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b335-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3b335-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="3b335-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b335-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="3b335-115">Not supported.</span></span>|
|<span data-ttu-id="3b335-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="3b335-116">Application</span></span>|<span data-ttu-id="3b335-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b335-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b335-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="3b335-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="3b335-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="3b335-119">Request headers</span></span>
|<span data-ttu-id="3b335-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="3b335-120">Header</span></span>|<span data-ttu-id="3b335-121">Valor</span><span class="sxs-lookup"><span data-stu-id="3b335-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b335-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="3b335-122">Authorization</span></span>|<span data-ttu-id="3b335-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="3b335-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b335-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="3b335-124">Accept</span></span>|<span data-ttu-id="3b335-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3b335-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b335-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="3b335-126">Request body</span></span>
<span data-ttu-id="3b335-127">No corpo da solicitação, forneça uma representação JSON do objeto managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="3b335-127">In the request body, supply a JSON representation for the managedIOSLobApp object.</span></span>

<span data-ttu-id="3b335-128">A tabela a seguir mostra as propriedades obrigatórias ao criar managedIOSLobApp.</span><span class="sxs-lookup"><span data-stu-id="3b335-128">The following table shows the properties that are required when you create the managedIOSLobApp.</span></span>

|<span data-ttu-id="3b335-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="3b335-129">Property</span></span>|<span data-ttu-id="3b335-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="3b335-130">Type</span></span>|<span data-ttu-id="3b335-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="3b335-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b335-132">id</span><span class="sxs-lookup"><span data-stu-id="3b335-132">id</span></span>|<span data-ttu-id="3b335-133">String</span><span class="sxs-lookup"><span data-stu-id="3b335-133">String</span></span>|<span data-ttu-id="3b335-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="3b335-134">Key of the entity.</span></span> <span data-ttu-id="3b335-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b335-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b335-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3b335-136">displayName</span></span>|<span data-ttu-id="3b335-137">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b335-137">String</span></span>|<span data-ttu-id="3b335-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="3b335-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="3b335-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b335-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b335-140">description</span><span class="sxs-lookup"><span data-stu-id="3b335-140">description</span></span>|<span data-ttu-id="3b335-141">String</span><span class="sxs-lookup"><span data-stu-id="3b335-141">String</span></span>|<span data-ttu-id="3b335-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3b335-142">The description of the app.</span></span> <span data-ttu-id="3b335-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b335-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b335-144">publicador</span><span class="sxs-lookup"><span data-stu-id="3b335-144">publisher</span></span>|<span data-ttu-id="3b335-145">String</span><span class="sxs-lookup"><span data-stu-id="3b335-145">String</span></span>|<span data-ttu-id="3b335-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3b335-146">The publisher of the app.</span></span> <span data-ttu-id="3b335-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b335-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b335-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="3b335-148">largeIcon</span></span>|[<span data-ttu-id="3b335-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="3b335-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="3b335-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="3b335-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="3b335-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b335-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b335-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3b335-152">createdDateTime</span></span>|<span data-ttu-id="3b335-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b335-153">DateTimeOffset</span></span>|<span data-ttu-id="3b335-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3b335-154">The date and time the app was created.</span></span> <span data-ttu-id="3b335-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b335-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b335-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3b335-156">lastModifiedDateTime</span></span>|<span data-ttu-id="3b335-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b335-157">DateTimeOffset</span></span>|<span data-ttu-id="3b335-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="3b335-158">The date and time the app was last modified.</span></span> <span data-ttu-id="3b335-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b335-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b335-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="3b335-160">isFeatured</span></span>|<span data-ttu-id="3b335-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b335-161">Boolean</span></span>|<span data-ttu-id="3b335-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b335-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b335-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="3b335-163">privacyInformationUrl</span></span>|<span data-ttu-id="3b335-164">String</span><span class="sxs-lookup"><span data-stu-id="3b335-164">String</span></span>|<span data-ttu-id="3b335-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="3b335-165">The privacy statement Url.</span></span> <span data-ttu-id="3b335-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b335-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b335-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="3b335-167">informationUrl</span></span>|<span data-ttu-id="3b335-168">String</span><span class="sxs-lookup"><span data-stu-id="3b335-168">String</span></span>|<span data-ttu-id="3b335-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="3b335-169">The more information Url.</span></span> <span data-ttu-id="3b335-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b335-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b335-171">owner</span><span class="sxs-lookup"><span data-stu-id="3b335-171">owner</span></span>|<span data-ttu-id="3b335-172">String</span><span class="sxs-lookup"><span data-stu-id="3b335-172">String</span></span>|<span data-ttu-id="3b335-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="3b335-173">The owner of the app.</span></span> <span data-ttu-id="3b335-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b335-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b335-175">developer</span><span class="sxs-lookup"><span data-stu-id="3b335-175">developer</span></span>|<span data-ttu-id="3b335-176">String</span><span class="sxs-lookup"><span data-stu-id="3b335-176">String</span></span>|<span data-ttu-id="3b335-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3b335-177">The developer of the app.</span></span> <span data-ttu-id="3b335-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b335-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b335-179">notes</span><span class="sxs-lookup"><span data-stu-id="3b335-179">notes</span></span>|<span data-ttu-id="3b335-180">String</span><span class="sxs-lookup"><span data-stu-id="3b335-180">String</span></span>|<span data-ttu-id="3b335-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3b335-181">Notes for the app.</span></span> <span data-ttu-id="3b335-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b335-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="3b335-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="3b335-183">publishingState</span></span>|[<span data-ttu-id="3b335-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="3b335-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="3b335-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3b335-185">The publishing state for the app.</span></span> <span data-ttu-id="3b335-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="3b335-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="3b335-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b335-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="3b335-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="3b335-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="3b335-189">appAvailability</span><span class="sxs-lookup"><span data-stu-id="3b335-189">appAvailability</span></span>|[<span data-ttu-id="3b335-190">managedAppAvailability</span><span class="sxs-lookup"><span data-stu-id="3b335-190">managedAppAvailability</span></span>](../resources/intune-apps-managedappavailability.md)|<span data-ttu-id="3b335-191">A disponibilidade do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3b335-191">The Application's availability.</span></span> <span data-ttu-id="3b335-192">Herdado de [managedApp](../resources/intune-apps-managedapp.md).</span><span class="sxs-lookup"><span data-stu-id="3b335-192">Inherited from [managedApp](../resources/intune-apps-managedapp.md).</span></span> <span data-ttu-id="3b335-193">Os valores possíveis são: `global`, `lineOfBusiness`.</span><span class="sxs-lookup"><span data-stu-id="3b335-193">Possible values are: `global`, `lineOfBusiness`.</span></span>|
|<span data-ttu-id="3b335-194">version</span><span class="sxs-lookup"><span data-stu-id="3b335-194">version</span></span>|<span data-ttu-id="3b335-195">Cadeia de caracteres</span><span class="sxs-lookup"><span data-stu-id="3b335-195">String</span></span>|<span data-ttu-id="3b335-196">A versão do Aplicativo.</span><span class="sxs-lookup"><span data-stu-id="3b335-196">The Application's version.</span></span> <span data-ttu-id="3b335-197">Herdado de [managedApp](../resources/intune-apps-managedapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b335-197">Inherited from [managedApp](../resources/intune-apps-managedapp.md)</span></span>|
|<span data-ttu-id="3b335-198">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="3b335-198">committedContentVersion</span></span>|<span data-ttu-id="3b335-199">String</span><span class="sxs-lookup"><span data-stu-id="3b335-199">String</span></span>|<span data-ttu-id="3b335-200">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="3b335-200">The internal committed content version.</span></span> <span data-ttu-id="3b335-201">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b335-201">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="3b335-202">fileName</span><span class="sxs-lookup"><span data-stu-id="3b335-202">fileName</span></span>|<span data-ttu-id="3b335-203">String</span><span class="sxs-lookup"><span data-stu-id="3b335-203">String</span></span>|<span data-ttu-id="3b335-204">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="3b335-204">The name of the main Lob application file.</span></span> <span data-ttu-id="3b335-205">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b335-205">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="3b335-206">size</span><span class="sxs-lookup"><span data-stu-id="3b335-206">size</span></span>|<span data-ttu-id="3b335-207">Int64</span><span class="sxs-lookup"><span data-stu-id="3b335-207">Int64</span></span>|<span data-ttu-id="3b335-208">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="3b335-208">The total size, including all uploaded files.</span></span> <span data-ttu-id="3b335-209">Herdado de [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="3b335-209">Inherited from [managedMobileLobApp](../resources/intune-apps-managedmobilelobapp.md)</span></span>|
|<span data-ttu-id="3b335-210">bundleId</span><span class="sxs-lookup"><span data-stu-id="3b335-210">bundleId</span></span>|<span data-ttu-id="3b335-211">String</span><span class="sxs-lookup"><span data-stu-id="3b335-211">String</span></span>|<span data-ttu-id="3b335-212">O Nome da Identidade.</span><span class="sxs-lookup"><span data-stu-id="3b335-212">The Identity Name.</span></span>|
|<span data-ttu-id="3b335-213">applicableDeviceType</span><span class="sxs-lookup"><span data-stu-id="3b335-213">applicableDeviceType</span></span>|[<span data-ttu-id="3b335-214">iosDeviceType</span><span class="sxs-lookup"><span data-stu-id="3b335-214">iosDeviceType</span></span>](../resources/intune-apps-iosdevicetype.md)|<span data-ttu-id="3b335-215">A arquitetura do iOS na qual esse aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="3b335-215">The iOS architecture for which this app can run on.</span></span>|
|<span data-ttu-id="3b335-216">minimumSupportedOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3b335-216">minimumSupportedOperatingSystem</span></span>|[<span data-ttu-id="3b335-217">iosMinimumOperatingSystem</span><span class="sxs-lookup"><span data-stu-id="3b335-217">iosMinimumOperatingSystem</span></span>](../resources/intune-apps-iosminimumoperatingsystem.md)|<span data-ttu-id="3b335-218">O valor do sistema de operacional mínimo aplicável.</span><span class="sxs-lookup"><span data-stu-id="3b335-218">The value for the minimum applicable operating system.</span></span>|
|<span data-ttu-id="3b335-219">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="3b335-219">expirationDateTime</span></span>|<span data-ttu-id="3b335-220">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b335-220">DateTimeOffset</span></span>|<span data-ttu-id="3b335-221">O tempo de expiração.</span><span class="sxs-lookup"><span data-stu-id="3b335-221">The expiration time.</span></span>|
|<span data-ttu-id="3b335-222">versionNumber</span><span class="sxs-lookup"><span data-stu-id="3b335-222">versionNumber</span></span>|<span data-ttu-id="3b335-223">String</span><span class="sxs-lookup"><span data-stu-id="3b335-223">String</span></span>|<span data-ttu-id="3b335-224">O número de versão do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="3b335-224">The version number of managed iOS Line of Business (LoB) app.</span></span>|
|<span data-ttu-id="3b335-225">buildNumber</span><span class="sxs-lookup"><span data-stu-id="3b335-225">buildNumber</span></span>|<span data-ttu-id="3b335-226">String</span><span class="sxs-lookup"><span data-stu-id="3b335-226">String</span></span>|<span data-ttu-id="3b335-227">O número de build do aplicativo gerenciado de Linha de Negócios (LoB) iOS gerenciado.</span><span class="sxs-lookup"><span data-stu-id="3b335-227">The build number of managed iOS Line of Business (LoB) app.</span></span>|



## <a name="response"></a><span data-ttu-id="3b335-228">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b335-228">Response</span></span>
<span data-ttu-id="3b335-229">Se tiver êxito, este método retornará o código de resposta `201 Created` e o objeto [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="3b335-229">If successful, this method returns a `201 Created` response code and a [managedIOSLobApp](../resources/intune-apps-managedioslobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b335-230">Exemplo</span><span class="sxs-lookup"><span data-stu-id="3b335-230">Example</span></span>

### <a name="request"></a><span data-ttu-id="3b335-231">Solicitação</span><span class="sxs-lookup"><span data-stu-id="3b335-231">Request</span></span>
<span data-ttu-id="3b335-232">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="3b335-232">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3b335-233">Resposta</span><span class="sxs-lookup"><span data-stu-id="3b335-233">Response</span></span>
<span data-ttu-id="3b335-p120">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="3b335-p120">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






