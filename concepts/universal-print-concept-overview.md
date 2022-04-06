---
title: Visão geral da API de impressão em nuvem da Impressão Universal
description: A Impressão Universal é uma solução moderna que as organizações podem usar para gerir a infraestrutura de impressão através de serviços de nuvem da Microsoft.
author: braedenp-msft
ms.localizationpriority: high
ms.prod: cloud-printing
ms.custom: scenarios:getting-started
ms.openlocfilehash: c66e967a4844226af29fecbcb1d6a9be2f47a2be
ms.sourcegitcommit: 43a7c971a97ce1e4c55cbae089820bfce7dfe42b
ms.translationtype: HT
ms.contentlocale: pt-BR
ms.lasthandoff: 03/29/2022
ms.locfileid: "64510243"
---
# <a name="universal-print-cloud-printing-api-overview"></a>Visão geral da API de impressão em nuvem da Impressão Universal

A Impressão Universal é uma solução moderna que as organizações podem usar para gerir a infraestrutura de impressão através de serviços de nuvem da Microsoft.

![Captura de tela da página inicial do portal da Impressão Universal do Azure](images/universal-print-portal-homepage.png)

## <a name="why-use-universal-print"></a>Por que usar a Impressão Universal?

A Impressão Universal move a funcionalidade de impressão do Windows Server para a nuvem do Microsoft 365, para que as organizações não precisem mais de servidores de impressão locais e não precisem instalar drivers de impressora em dispositivos. Além disso, a Impressão Universal adiciona funcionalidades fundamentais, como grupos de segurança para acesso à impressora, descoberta de impressora baseada no local e uma experiência de administrador avançada.

Como as organizações adotam a Impressão Universal, as organizações e os fornecedores independentes de software (ISVs) podem usar a API de Impressão Universal no Microsoft Graph para criar e ampliar aplicativos para suportar novos cenários.

### <a name="print-documents-from-web-and-mobile-applications"></a>Imprimir documentos de aplicativos da Web e móveis

Mover a infraestrutura de impressão para a nuvem permite imprimir documentos diretamente de aplicativos da Web e móveis.
- Os usuários podem enviar trabalhos de impressão para o printerShare.
- Os administradores da impressora também podem enviar trabalhos de impressão, para fazer testes preliminares antes de compartilhar a impressora com a organização.

Siga estas etapas para enviar trabalhos de impressão para o printerShare:

1. [Crie um trabalho de impressão](/graph/api/printershare-post-jobs) e armazene a ID do documento resultante.
2. [Crie uma uploadSession](/graph/api/printdocument-createuploadsession) para o documento. 
3. [Bytes de upload para a sessão de upload criada](./upload-data-to-upload-session.md).
4. [Iniciar o trabalho de impressão](/graph/api/printjob-start).

### <a name="manage-printers"></a>Gerenciar impressoras

É uma tarefa complexa acompanhar as impressoras de uma organização, suas configurações e uso. A API de Impressão Universal permite a integração em todas as três áreas.

* **Fique de olho no estado, configurações e disponibilidade da impressora**, usando a [Lista de impressoras](/graph/api/print-list-printers) e o [printerStatus](/graph/api/resources/printerstatus).

* **Veja quem está usando as impressoras e o quanto elas estão imprimindo** usando as APIs de relatórios:
  * [Listar dailyPrintUsageByUser](/graph/api/reportroot-list-dailyprintusagebyuser)
  * [Listar monthlyPrintUsageByUser](/graph/api/reportroot-list-monthlyprintusagebyuser)
  * [Listar dailyPrintUsageByPrinter](/graph/api/reportroot-list-dailyprintusagebyprinter)
  * [Listar monthlyPrintUsageByPrinter](/graph/api/reportroot-list-monthlyprintusagebyprinter)

* **Configurar permissões de usuário** modificando a associação de usuários e grupos das impressoras:
  * [Listar allowedUsers](/graph/api/printershare-list-allowedusers)
  * [Adicionar allowedUser](/graph/api/printershare-post-allowedusers)
  * [Remover allowedUser](/graph/api/printershare-delete-alloweduser)
  * [Listar allowedGroups](/graph/api/printershare-list-allowedgroups)
  * [Adicionar allowedGroup](/graph/api/printershare-post-allowedgroups)
  * [Remover allowedGroup](/graph/api/printershare-delete-allowedgroup)

### <a name="seamlessly-replace-or-update-printer-hardware"></a>Substituir ou atualizar o hardware da impressora sem problemas

As impressoras não estarão visíveis para os usuários até que sejam [compartilhadas](/graph/api/print-post-shares), proporcionando aos administradores um controle detalhado sobre qual hardware de impressora estará disponível em um determinado momento.

O compartilhamento de uma impressora cria um recurso [printerShare](/graph/api/resources/printershare) que pode ser atualizado a qualquer momento para indicar uma impressora diferente, facilitando a substituição de hardware de uma impressora quebrada ou a desativação de impressoras para manutenção.

Para usá-lo em seu aplicativo, use [Update printerShare](/graph/api/printershare-update) para atualizar a referência `printer` de printerShare.

### <a name="extending-universal-print-to-support-pull-printing"></a>Extensão da Impressão Universal para suporte à impressão segura

A API de Impressão Universal do Microsoft Graph permite que o seu aplicativo suporte a impressão segura. Para configurar a impressão segura, você registrará acionadores que notificarão o seu aplicativo (via comunicação serviço a serviço) quando determinados eventos de impressão acontecem, como um trabalho de impressão sendo iniciado.

Esses acionadores permitem que o seu aplicativo interrompa o fluxo de trabalho de impressão para fazer coisas como redirecionar os trabalhos para diferentes impressoras e modificar o conteúdo do documento.

Siga estes passos para habilitar a impressão segura:

1. [Crie uma Definição de Tarefa de impressão](/graph/api/print-post-taskdefinitions) usando as permissões do aplicativo. Esta definição de tarefa abstrata será usada para criar a tarefa que irá realizar o trabalho para o seu aplicativo. É necessário estabelecer pelo menos uma definição de tarefa por inquilino, que pode ser associada a qualquer número de impressoras, usando acionadores de tarefa (ver etapa 4).

2. [Registre uma ou mais impressoras virtuais](/graph/api/printer-create) usando um token de autenticação de administrador e um `null` **Dispositivo físico**. Sem um dispositivo físico acoplado, uma "impressora virtual" é apenas um objeto de impressora na Impressão Universal. Normalmente, os usuários imprimem em impressoras virtuais e depois pegam seus trabalhos de impressão em um dispositivo físico de impressão. Veja o passo 6.

3. [Atualize os atributos de sua impressora virtual](/graph/api/printer-update) usando as permissões do aplicativo e um `application/ipp` tipo de mídia (veja exemplos).

4. [Crie um acionador de tarefas para sua impressora virtual](/graph/api/printer-post-tasktriggers) usando um token de autenticação de administrador que irá associar a definição da sua tarefa com a impressora virtual.

5. Quando um trabalho de impressão é enviado para a impressora virtual, ele será pausado devido ao [ Acionador de Tarefas de impressão](/graph/api/resources/printtasktrigger). Uma [Tarefa de impressão](/graph/api/resources/printtask) com `processing`estado será criada com base na [Definição da Tarefa de impressão associada](/graph/api/resources/printtaskdefinition).

6. Quando o usuário passar um crachá em um dispositivo físico de impressão, a impressora notificará o seu aplicativo. Nessa altura, o seu aplicativo pode [buscar os trabalhos da impressora virtual associada](/graph/api/printer-list-jobs) e filtrar a lista de trabalhos criados pelo usuário atual.

7. Quando o usuário seleciona um ou mais trabalhos para imprimir, seu aplicativo pode [redirecionar o(s) trabalho(s) de impressão](/graph/api/printjob-redirect) para a impressora física e o trabalho começará a imprimir! A chamada de redirecionamento só terá sucesso se houver uma [Tarefa de impressão](/graph/api/resources/printtask) em `processing` estado na impressora associada iniciada por um acionador que este aplicativo criou no passo 4. A tarefa será automaticamente definida para o `completed` estado após o redirecionamento.

## <a name="api-reference"></a>Referência da API
Está procurando a referência de API para esse serviço?

- [Impressão Universal API no Microsoft Graph](/graph/api/resources/print)

## <a name="provide-feedback"></a>Faça comentários

Gostaríamos de ouvir seus comentários sobre as APIs de Impressão Universal. Forneça suas sugestões no fórum de ideias da[Plataforma de Desenvolvedor do Microsoft 365](https://techcommunity.microsoft.com/t5/microsoft-365-developer-platform/idb-p/Microsoft365DeveloperPlatform/label-name/Microsoft%20Graph).

## <a name="see-also"></a>Confira também

- [O que é a impressão universal?](/universal-print/fundamentals/universal-print-whatis)
