import fastifyAccepts from '@fastify/accepts';
import fastifySwagger from '@fastify/swagger';
import fastifySwaggerUI from '@fastify/swagger-ui';
import type { TypeBoxTypeProvider } from '@fastify/type-provider-typebox';
import { GrowthBook } from '@growthbook/growthbook';
import Ajv from 'ajv';
import addFormats from 'ajv-formats';
import uriResolver from 'fast-uri';
import Fastify, {
  FastifyBaseLogger,
  FastifyHttpOptions,
  FastifyInstance,
  RawReplyDefaultExpression,
  RawRequestDefaultExpression,
  RawServerDefault
} from 'fastify';

import prismaPlugin from './db/prisma';
import cookies from './plugins/cookies';
import cors from './plugins/cors';
import { NodemailerProvider } from './plugins/mail-providers/nodemailer';
import { SESProvider } from './plugins/mail-providers/ses';
import mailer from './plugins/mailer';
import redirectWithMessage from './plugins/redirect-with-message';
import security from './plugins/security';
import auth from './plugins/auth';
import bouncer from './plugins/bouncer';
import errorHandling from './plugins/error-handling';
import csrf from './plugins/csrf';
import notFound from './plugins/not-found';
import shadowCapture from './plugins/shadow-capture';
import growthBook from './plugins/growth-book';

- 👋 Hi, I’m @tadese-ayane
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
tadese-ayane/tadese-ayane is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
