---
title: Atualizar win32LobApp
description: Atualize as propriedades de um objeto win32LobApp.
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b7c3a48d9c8e982087c5306e7c60db34c5612108
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: pt-BR
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757287"
---
# <a name="update-win32lobapp"></a><span data-ttu-id="a6a3b-103">Atualizar win32LobApp</span><span class="sxs-lookup"><span data-stu-id="a6a3b-103">Update win32LobApp</span></span>

<span data-ttu-id="a6a3b-104">Namespace: microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6a3b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a6a3b-105">**Observação:** A API do Microsoft Graph para Intune requer uma [licença ativa do Intune](https://go.microsoft.com/fwlink/?linkid=839381) para o locatário.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a6a3b-106">Atualize as propriedades de um [objeto win32LobApp.](../resources/intune-apps-win32lobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a6a3b-106">Update the properties of a [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a6a3b-107">Pré-requisitos</span><span class="sxs-lookup"><span data-stu-id="a6a3b-107">Prerequisites</span></span>
<span data-ttu-id="a6a3b-p101">Uma das seguintes permissões é obrigatória para chamar esta API. Para saber mais, incluindo como escolher permissões, confira [Permissões](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="a6a3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a6a3b-110">Tipo de permissão</span><span class="sxs-lookup"><span data-stu-id="a6a3b-110">Permission type</span></span>|<span data-ttu-id="a6a3b-111">Permissões (da com menos para a com mais privilégios)</span><span class="sxs-lookup"><span data-stu-id="a6a3b-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6a3b-112">Delegado (conta corporativa ou de estudante)</span><span class="sxs-lookup"><span data-stu-id="a6a3b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a6a3b-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6a3b-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a6a3b-114">Delegado (conta pessoal da Microsoft)</span><span class="sxs-lookup"><span data-stu-id="a6a3b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6a3b-115">Sem suporte.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-115">Not supported.</span></span>|
|<span data-ttu-id="a6a3b-116">Aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6a3b-116">Application</span></span>|<span data-ttu-id="a6a3b-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6a3b-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6a3b-118">Solicitação HTTP</span><span class="sxs-lookup"><span data-stu-id="a6a3b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}
```

## <a name="request-headers"></a><span data-ttu-id="a6a3b-119">Cabeçalhos de solicitação</span><span class="sxs-lookup"><span data-stu-id="a6a3b-119">Request headers</span></span>
|<span data-ttu-id="a6a3b-120">Cabeçalho</span><span class="sxs-lookup"><span data-stu-id="a6a3b-120">Header</span></span>|<span data-ttu-id="a6a3b-121">Valor</span><span class="sxs-lookup"><span data-stu-id="a6a3b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6a3b-122">Autorização</span><span class="sxs-lookup"><span data-stu-id="a6a3b-122">Authorization</span></span>|<span data-ttu-id="a6a3b-123">&lt;Token&gt; de portador obrigatório.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6a3b-124">Aceitar</span><span class="sxs-lookup"><span data-stu-id="a6a3b-124">Accept</span></span>|<span data-ttu-id="a6a3b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a6a3b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6a3b-126">Corpo da solicitação</span><span class="sxs-lookup"><span data-stu-id="a6a3b-126">Request body</span></span>
<span data-ttu-id="a6a3b-127">No corpo da solicitação, fornece uma representação JSON para o [objeto win32LobApp.](../resources/intune-apps-win32lobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a6a3b-127">In the request body, supply a JSON representation for the [win32LobApp](../resources/intune-apps-win32lobapp.md) object.</span></span>

<span data-ttu-id="a6a3b-128">A tabela a seguir mostra as propriedades que são necessárias ao criar [o win32LobApp](../resources/intune-apps-win32lobapp.md).</span><span class="sxs-lookup"><span data-stu-id="a6a3b-128">The following table shows the properties that are required when you create the [win32LobApp](../resources/intune-apps-win32lobapp.md).</span></span>

|<span data-ttu-id="a6a3b-129">Propriedade</span><span class="sxs-lookup"><span data-stu-id="a6a3b-129">Property</span></span>|<span data-ttu-id="a6a3b-130">Tipo</span><span class="sxs-lookup"><span data-stu-id="a6a3b-130">Type</span></span>|<span data-ttu-id="a6a3b-131">Descrição</span><span class="sxs-lookup"><span data-stu-id="a6a3b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6a3b-132">id</span><span class="sxs-lookup"><span data-stu-id="a6a3b-132">id</span></span>|<span data-ttu-id="a6a3b-133">String</span><span class="sxs-lookup"><span data-stu-id="a6a3b-133">String</span></span>|<span data-ttu-id="a6a3b-134">Chave da entidade.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-134">Key of the entity.</span></span> <span data-ttu-id="a6a3b-135">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a6a3b-135">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a3b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a6a3b-136">displayName</span></span>|<span data-ttu-id="a6a3b-137">String</span><span class="sxs-lookup"><span data-stu-id="a6a3b-137">String</span></span>|<span data-ttu-id="a6a3b-138">O título do aplicativo importado ou definido pelo administrador.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-138">The admin provided or imported title of the app.</span></span> <span data-ttu-id="a6a3b-139">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a6a3b-139">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a3b-140">description</span><span class="sxs-lookup"><span data-stu-id="a6a3b-140">description</span></span>|<span data-ttu-id="a6a3b-141">String</span><span class="sxs-lookup"><span data-stu-id="a6a3b-141">String</span></span>|<span data-ttu-id="a6a3b-142">A descrição do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-142">The description of the app.</span></span> <span data-ttu-id="a6a3b-143">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a6a3b-143">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a3b-144">publicador</span><span class="sxs-lookup"><span data-stu-id="a6a3b-144">publisher</span></span>|<span data-ttu-id="a6a3b-145">String</span><span class="sxs-lookup"><span data-stu-id="a6a3b-145">String</span></span>|<span data-ttu-id="a6a3b-146">O publicador do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-146">The publisher of the app.</span></span> <span data-ttu-id="a6a3b-147">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a6a3b-147">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a3b-148">largeIcon</span><span class="sxs-lookup"><span data-stu-id="a6a3b-148">largeIcon</span></span>|[<span data-ttu-id="a6a3b-149">mimeContent</span><span class="sxs-lookup"><span data-stu-id="a6a3b-149">mimeContent</span></span>](../resources/intune-shared-mimecontent.md)|<span data-ttu-id="a6a3b-150">O ícone grande, a ser exibido nos detalhes do aplicativo e usado para o carregamento do ícone.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-150">The large icon, to be displayed in the app details and used for upload of the icon.</span></span> <span data-ttu-id="a6a3b-151">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a6a3b-151">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a3b-152">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a6a3b-152">createdDateTime</span></span>|<span data-ttu-id="a6a3b-153">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6a3b-153">DateTimeOffset</span></span>|<span data-ttu-id="a6a3b-154">A data e a hora da criação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-154">The date and time the app was created.</span></span> <span data-ttu-id="a6a3b-155">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a6a3b-155">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a3b-156">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a6a3b-156">lastModifiedDateTime</span></span>|<span data-ttu-id="a6a3b-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a6a3b-157">DateTimeOffset</span></span>|<span data-ttu-id="a6a3b-158">A data e a hora que o aplicativo foi modificado pela última vez.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-158">The date and time the app was last modified.</span></span> <span data-ttu-id="a6a3b-159">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a6a3b-159">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a3b-160">isFeatured</span><span class="sxs-lookup"><span data-stu-id="a6a3b-160">isFeatured</span></span>|<span data-ttu-id="a6a3b-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="a6a3b-161">Boolean</span></span>|<span data-ttu-id="a6a3b-162">O valor que indica se o aplicativo está marcado como em destaque pelo administrador. Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a6a3b-162">The value indicating whether the app is marked as featured by the admin. Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a3b-163">privacyInformationUrl</span><span class="sxs-lookup"><span data-stu-id="a6a3b-163">privacyInformationUrl</span></span>|<span data-ttu-id="a6a3b-164">String</span><span class="sxs-lookup"><span data-stu-id="a6a3b-164">String</span></span>|<span data-ttu-id="a6a3b-165">A URL da declaração de privacidade.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-165">The privacy statement Url.</span></span> <span data-ttu-id="a6a3b-166">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a6a3b-166">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a3b-167">informationUrl</span><span class="sxs-lookup"><span data-stu-id="a6a3b-167">informationUrl</span></span>|<span data-ttu-id="a6a3b-168">String</span><span class="sxs-lookup"><span data-stu-id="a6a3b-168">String</span></span>|<span data-ttu-id="a6a3b-169">A URL de informações adicionais.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-169">The more information Url.</span></span> <span data-ttu-id="a6a3b-170">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a6a3b-170">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a3b-171">proprietário</span><span class="sxs-lookup"><span data-stu-id="a6a3b-171">owner</span></span>|<span data-ttu-id="a6a3b-172">String</span><span class="sxs-lookup"><span data-stu-id="a6a3b-172">String</span></span>|<span data-ttu-id="a6a3b-173">O proprietário do conteúdo.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-173">The owner of the app.</span></span> <span data-ttu-id="a6a3b-174">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a6a3b-174">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a3b-175">developer</span><span class="sxs-lookup"><span data-stu-id="a6a3b-175">developer</span></span>|<span data-ttu-id="a6a3b-176">String</span><span class="sxs-lookup"><span data-stu-id="a6a3b-176">String</span></span>|<span data-ttu-id="a6a3b-177">O desenvolvedor do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-177">The developer of the app.</span></span> <span data-ttu-id="a6a3b-178">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a6a3b-178">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a3b-179">notes</span><span class="sxs-lookup"><span data-stu-id="a6a3b-179">notes</span></span>|<span data-ttu-id="a6a3b-180">String</span><span class="sxs-lookup"><span data-stu-id="a6a3b-180">String</span></span>|<span data-ttu-id="a6a3b-181">Anotações do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-181">Notes for the app.</span></span> <span data-ttu-id="a6a3b-182">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md)</span><span class="sxs-lookup"><span data-stu-id="a6a3b-182">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md)</span></span>|
|<span data-ttu-id="a6a3b-183">publishingState</span><span class="sxs-lookup"><span data-stu-id="a6a3b-183">publishingState</span></span>|[<span data-ttu-id="a6a3b-184">mobileAppPublishingState</span><span class="sxs-lookup"><span data-stu-id="a6a3b-184">mobileAppPublishingState</span></span>](../resources/intune-apps-mobileapppublishingstate.md)|<span data-ttu-id="a6a3b-185">O estado de publicação do aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-185">The publishing state for the app.</span></span> <span data-ttu-id="a6a3b-186">O aplicativo não pode ser assinado, a menos que ele seja publicado.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-186">The app cannot be assigned unless the app is published.</span></span> <span data-ttu-id="a6a3b-187">Herdado de [mobileApp](../resources/intune-apps-mobileapp.md).</span><span class="sxs-lookup"><span data-stu-id="a6a3b-187">Inherited from [mobileApp](../resources/intune-apps-mobileapp.md).</span></span> <span data-ttu-id="a6a3b-188">Os valores possíveis são: `notPublished`, `processing`, `published`.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-188">Possible values are: `notPublished`, `processing`, `published`.</span></span>|
|<span data-ttu-id="a6a3b-189">committedContentVersion</span><span class="sxs-lookup"><span data-stu-id="a6a3b-189">committedContentVersion</span></span>|<span data-ttu-id="a6a3b-190">String</span><span class="sxs-lookup"><span data-stu-id="a6a3b-190">String</span></span>|<span data-ttu-id="a6a3b-191">A versão do conteúdo interno confirmado.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-191">The internal committed content version.</span></span> <span data-ttu-id="a6a3b-192">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a6a3b-192">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a6a3b-193">fileName</span><span class="sxs-lookup"><span data-stu-id="a6a3b-193">fileName</span></span>|<span data-ttu-id="a6a3b-194">String</span><span class="sxs-lookup"><span data-stu-id="a6a3b-194">String</span></span>|<span data-ttu-id="a6a3b-195">O nome do arquivo do aplicativo Lob principal.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-195">The name of the main Lob application file.</span></span> <span data-ttu-id="a6a3b-196">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a6a3b-196">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a6a3b-197">size</span><span class="sxs-lookup"><span data-stu-id="a6a3b-197">size</span></span>|<span data-ttu-id="a6a3b-198">Int64</span><span class="sxs-lookup"><span data-stu-id="a6a3b-198">Int64</span></span>|<span data-ttu-id="a6a3b-199">O tamanho total, incluindo todos os arquivos carregados.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-199">The total size, including all uploaded files.</span></span> <span data-ttu-id="a6a3b-200">Herdado de [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span><span class="sxs-lookup"><span data-stu-id="a6a3b-200">Inherited from [mobileLobApp](../resources/intune-apps-mobilelobapp.md)</span></span>|
|<span data-ttu-id="a6a3b-201">installCommandLine</span><span class="sxs-lookup"><span data-stu-id="a6a3b-201">installCommandLine</span></span>|<span data-ttu-id="a6a3b-202">String</span><span class="sxs-lookup"><span data-stu-id="a6a3b-202">String</span></span>|<span data-ttu-id="a6a3b-203">A linha de comando para instalar este aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6a3b-203">The command line to install this app</span></span>|
|<span data-ttu-id="a6a3b-204">uninstallCommandLine</span><span class="sxs-lookup"><span data-stu-id="a6a3b-204">uninstallCommandLine</span></span>|<span data-ttu-id="a6a3b-205">String</span><span class="sxs-lookup"><span data-stu-id="a6a3b-205">String</span></span>|<span data-ttu-id="a6a3b-206">A linha de comando para desinstalar esse aplicativo</span><span class="sxs-lookup"><span data-stu-id="a6a3b-206">The command line to uninstall this app</span></span>|
|<span data-ttu-id="a6a3b-207">applicableArchitectures</span><span class="sxs-lookup"><span data-stu-id="a6a3b-207">applicableArchitectures</span></span>|[<span data-ttu-id="a6a3b-208">windowsArchitecture</span><span class="sxs-lookup"><span data-stu-id="a6a3b-208">windowsArchitecture</span></span>](../resources/intune-apps-windowsarchitecture.md)|<span data-ttu-id="a6a3b-209">As arquiteturas do Windows nas quais este aplicativo pode ser executado.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-209">The Windows architecture(s) for which this app can run on.</span></span> <span data-ttu-id="a6a3b-210">Os valores possíveis são: `none`, `x86`, `x64`, `arm`, `neutral`.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-210">Possible values are: `none`, `x86`, `x64`, `arm`, `neutral`.</span></span>|
|<span data-ttu-id="a6a3b-211">minimumFreeDiskSpaceInMB</span><span class="sxs-lookup"><span data-stu-id="a6a3b-211">minimumFreeDiskSpaceInMB</span></span>|<span data-ttu-id="a6a3b-212">Int32</span><span class="sxs-lookup"><span data-stu-id="a6a3b-212">Int32</span></span>|<span data-ttu-id="a6a3b-213">O valor do espaço em disco gratuito mínimo necessário para instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-213">The value for the minimum free disk space which is required to install this app.</span></span>|
|<span data-ttu-id="a6a3b-214">minimumMemoryInMB</span><span class="sxs-lookup"><span data-stu-id="a6a3b-214">minimumMemoryInMB</span></span>|<span data-ttu-id="a6a3b-215">Int32</span><span class="sxs-lookup"><span data-stu-id="a6a3b-215">Int32</span></span>|<span data-ttu-id="a6a3b-216">O valor da memória física mínima necessária para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-216">The value for the minimum physical memory which is required to install this app.</span></span>|
|<span data-ttu-id="a6a3b-217">minimumNumberOfProcessors</span><span class="sxs-lookup"><span data-stu-id="a6a3b-217">minimumNumberOfProcessors</span></span>|<span data-ttu-id="a6a3b-218">Int32</span><span class="sxs-lookup"><span data-stu-id="a6a3b-218">Int32</span></span>|<span data-ttu-id="a6a3b-219">O valor do número mínimo de processadores necessário para instalar esse aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-219">The value for the minimum number of processors which is required to install this app.</span></span>|
|<span data-ttu-id="a6a3b-220">minimumCpuSpeedInMHz</span><span class="sxs-lookup"><span data-stu-id="a6a3b-220">minimumCpuSpeedInMHz</span></span>|<span data-ttu-id="a6a3b-221">Int32</span><span class="sxs-lookup"><span data-stu-id="a6a3b-221">Int32</span></span>|<span data-ttu-id="a6a3b-222">O valor da velocidade mínima da CPU necessária para instalar este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-222">The value for the minimum CPU speed which is required to install this app.</span></span>|
|<span data-ttu-id="a6a3b-223">rules</span><span class="sxs-lookup"><span data-stu-id="a6a3b-223">rules</span></span>|<span data-ttu-id="a6a3b-224">[Coleção win32LobAppRule](../resources/intune-apps-win32lobapprule.md)</span><span class="sxs-lookup"><span data-stu-id="a6a3b-224">[win32LobAppRule](../resources/intune-apps-win32lobapprule.md) collection</span></span>|<span data-ttu-id="a6a3b-225">As regras de detecção e requisitos para este aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-225">The detection and requirement rules for this app.</span></span>|
|<span data-ttu-id="a6a3b-226">installExperience</span><span class="sxs-lookup"><span data-stu-id="a6a3b-226">installExperience</span></span>|[<span data-ttu-id="a6a3b-227">win32LobAppInstallExperience</span><span class="sxs-lookup"><span data-stu-id="a6a3b-227">win32LobAppInstallExperience</span></span>](../resources/intune-apps-win32lobappinstallexperience.md)|<span data-ttu-id="a6a3b-228">A experiência de instalação deste aplicativo.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-228">The install experience for this app.</span></span>|
|<span data-ttu-id="a6a3b-229">returnCodes</span><span class="sxs-lookup"><span data-stu-id="a6a3b-229">returnCodes</span></span>|<span data-ttu-id="a6a3b-230">[Coleção win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md)</span><span class="sxs-lookup"><span data-stu-id="a6a3b-230">[win32LobAppReturnCode](../resources/intune-apps-win32lobappreturncode.md) collection</span></span>|<span data-ttu-id="a6a3b-231">Os códigos de retorno para o comportamento pós-instalação.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-231">The return codes for post installation behavior.</span></span>|
|<span data-ttu-id="a6a3b-232">msiInformation</span><span class="sxs-lookup"><span data-stu-id="a6a3b-232">msiInformation</span></span>|[<span data-ttu-id="a6a3b-233">win32LobAppMsiInformation</span><span class="sxs-lookup"><span data-stu-id="a6a3b-233">win32LobAppMsiInformation</span></span>](../resources/intune-apps-win32lobappmsiinformation.md)|<span data-ttu-id="a6a3b-234">O MSI detalha se esse aplicativo Win32 é um aplicativo MSI.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-234">The MSI details if this Win32 app is an MSI app.</span></span>|
|<span data-ttu-id="a6a3b-235">setupFilePath</span><span class="sxs-lookup"><span data-stu-id="a6a3b-235">setupFilePath</span></span>|<span data-ttu-id="a6a3b-236">String</span><span class="sxs-lookup"><span data-stu-id="a6a3b-236">String</span></span>|<span data-ttu-id="a6a3b-237">O caminho relativo do arquivo de instalação no pacote Win32LobApp criptografado.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-237">The relative path of the setup file in the encrypted Win32LobApp package.</span></span>|
|<span data-ttu-id="a6a3b-238">minimumSupportedWindowsRelease</span><span class="sxs-lookup"><span data-stu-id="a6a3b-238">minimumSupportedWindowsRelease</span></span>|<span data-ttu-id="a6a3b-239">String</span><span class="sxs-lookup"><span data-stu-id="a6a3b-239">String</span></span>|<span data-ttu-id="a6a3b-240">O valor da versão mínima com suporte do Windows.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-240">The value for the minimum supported windows release.</span></span>|



## <a name="response"></a><span data-ttu-id="a6a3b-241">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6a3b-241">Response</span></span>
<span data-ttu-id="a6a3b-242">Se tiver êxito, este método retornará um código de resposta e um `200 OK` [objeto win32LobApp](../resources/intune-apps-win32lobapp.md) atualizado no corpo da resposta.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-242">If successful, this method returns a `200 OK` response code and an updated [win32LobApp](../resources/intune-apps-win32lobapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6a3b-243">Exemplo</span><span class="sxs-lookup"><span data-stu-id="a6a3b-243">Example</span></span>

### <a name="request"></a><span data-ttu-id="a6a3b-244">Solicitação</span><span class="sxs-lookup"><span data-stu-id="a6a3b-244">Request</span></span>
<span data-ttu-id="a6a3b-245">Este é um exemplo da solicitação.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-245">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}
Content-type: application/json
Content-length: 2134

{
  "@odata.type": "#microsoft.graph.win32LobApp",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
      "ruleType": "requirement",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "operationType": "exists",
      "operator": "equal",
      "comparisonValue": "Comparison Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value",
  "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value"
}
```

### <a name="response"></a><span data-ttu-id="a6a3b-246">Resposta</span><span class="sxs-lookup"><span data-stu-id="a6a3b-246">Response</span></span>
<span data-ttu-id="a6a3b-p119">Veja a seguir um exemplo da resposta. Observação: o objeto response mostrado aqui pode estar truncado por motivos de concisão. Todas as propriedades serão retornadas de uma chamada real.</span><span class="sxs-lookup"><span data-stu-id="a6a3b-p119">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2306

{
  "@odata.type": "#microsoft.graph.win32LobApp",
  "id": "9607b530-b530-9607-30b5-079630b50796",
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
  "committedContentVersion": "Committed Content Version value",
  "fileName": "File Name value",
  "size": 4,
  "installCommandLine": "Install Command Line value",
  "uninstallCommandLine": "Uninstall Command Line value",
  "applicableArchitectures": "x86",
  "minimumFreeDiskSpaceInMB": 8,
  "minimumMemoryInMB": 1,
  "minimumNumberOfProcessors": 9,
  "minimumCpuSpeedInMHz": 4,
  "rules": [
    {
      "@odata.type": "microsoft.graph.win32LobAppRegistryRule",
      "ruleType": "requirement",
      "check32BitOn64System": true,
      "keyPath": "Key Path value",
      "valueName": "Value Name value",
      "operationType": "exists",
      "operator": "equal",
      "comparisonValue": "Comparison Value value"
    }
  ],
  "installExperience": {
    "@odata.type": "microsoft.graph.win32LobAppInstallExperience",
    "runAsAccount": "user",
    "deviceRestartBehavior": "allow"
  },
  "returnCodes": [
    {
      "@odata.type": "microsoft.graph.win32LobAppReturnCode",
      "returnCode": 10,
      "type": "success"
    }
  ],
  "msiInformation": {
    "@odata.type": "microsoft.graph.win32LobAppMsiInformation",
    "productCode": "Product Code value",
    "productVersion": "Product Version value",
    "upgradeCode": "Upgrade Code value",
    "requiresReboot": true,
    "packageType": "perUser",
    "productName": "Product Name value",
    "publisher": "Publisher value"
  },
  "setupFilePath": "Setup File Path value",
  "minimumSupportedWindowsRelease": "Minimum Supported Windows Release value"
}
```




